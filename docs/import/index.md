---
sidebar_position: 3
---
# Import diagrams from json

Import menu allows to add json with diagrams into any project.

<img srcset="./import.png 2x" alt="Import menu"/>

## JSON format

Format desctiption is given as Type Script classes

```
class Diagram {
  id: string
  programName: string
  models: Model[]
  edges: Edge[]
  relations: Relation[]
  mappings: Mapping[]
}
```

```
class Model {
  id: string
  identifier: string
  type: 'usecase'
  color: 'string'
  x: number
  y: number
  vertices: Vertex[]
}
```

```
class Vertex {
  id: string
  value: string
  comment: string
  type: 'variable' | 'tuple' | 'choice' | 'subitem'
  x: number?
  y: number?
  decomposableMode: boolean
  vertices: Vertex[]
}
```

```
class Edge {
  id: string
  id1: string
  id2: string
  type: 'common' | 'mapping' | 'element-mapping' | 'linkToElement'
  decomposableMode: boolean
  textField: {
    id: string
    value: string
    comment: string
    decomposableMode: boolean
    relativeDirProj: number = 0.5
    shift: number = 0
    relativeNormProj: number | null = null
  }
}
```

```
class Relation {
  id: string
  value: string
  relationDirection: '=>' | '<=' | '<=>' | 'o'
  isCollapsed: boolean
  from: string[]
  to: string[]
}
```

```
class Mapping {
  id: string
  mappingEdgeId: string
  sourceId: string
  targetId: string
  mappingEdges: string[]
}
```