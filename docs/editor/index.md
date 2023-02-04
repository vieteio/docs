---
sidebar_position: 2
---
# Editor tutorial

This tutorial shows how to use editor on example of DAO economic model modeling task.

In context of DAO modeling task editor allows:
1. to describe general schema of DAO mechanics in a free mode

<img src="./useCaseAndGovernance.png" alt="DAO general schema" width="400"/>

2. to describe evaluation logic for metrics (for example token price) in a decomposable mode

<img src="./metricEvaluation.png" alt="Metirc evaluation" width="400"/>

3. to generate Python code for probabilistic modeling. The launched code will run modeling and display plots for selected metrics as the modeling result.

Below we will walk through how to create schemas in the editor, and as a result, we will draw the schemas of the Freelance DAO project, fragments of which are in the screenshots above.

## Create project

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To start draw a schema create a new project. Press button "Create project" a the top of the header.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./createProject.png 2x" alt="Create project"/>
</div>

<div style={{ width: '50%', clear: 'both' }}>
You will get an empty project. To draw anything in it add a model.
</div>

## Create model

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create a model open a context menu with a right mouse button click on any empty space and select menu item "Add model"
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addModel.png 2x" alt="Add model"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
The new model will be created
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newModel.png 2x" alt="New model"/>
</div>

<div style={{ width: '50%', clear: 'both' }}>
Now you can create objects and edges to draw a scheme.
</div>

## Create objects and edges

Vertices could be created only inside some model. Edges could be drawn between any objects (including objects from different models). 

> Also it is permitted to draw an edge from a object into an edge, but not reverse. More about this later.

### Create object

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create an object open a model context menu with a right mouse button click on any empty space *inside the model* and select menu item "Add object"
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addObject.png 2x" alt="Add object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
The new object will be created inside model.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newObject.png 2x" alt="New object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
You can put a text, for example an object's name, into the object. To do that click on the object with left mouse button. Cursor will appear.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./cursorInsideObject.png 2x" alt="Cursor inside an object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Enter any text. Only a single line of text is allowed.

To remove cursor click on any empty space of the editor or a model.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newObjectWithName.png 2x" alt="Object with a text inside"/>
</div>

<div style={{ width: '50%', clear: 'both' }}>
</div>

### Create edge

Let's create a first edge. Viete is aimed to create fast chains of objects connected by edges. So creating and edge requires minimum actions.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create an edge just drag it from an object. Click with left mouse button on an object and drag the mouse outside the object. Edge will appear with a start at the object and it's end will follow to the mouse.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./dragEdge.png 2x" alt="Dragging edge from an object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Release the mouse button and the edge will be created tohether with a new object for the edge's end.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newObjectAndEdge.png 2x" alt="Created edge with a new object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
You can enter a text on the new object.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newNamedObjectAndEdge.png 2x" alt="Created edge with a named end object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Also you could add text to the edge. To do that hover mouse on the edge and text field for the edge will appear
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./hoveredEdgeWithVisibleTextField.png 2x" alt="Hovered edge with a visible text field"/>
</div>


<div style={{ width: '50%', clear: 'both' }}>
</div>

1. Первые вершины и ребра
2. Tuple для описания состояний
3. Choice для описания альтернатив в сценариях
4. Атрибуты для описания параметров действий
5. Mapping для декларации переходов от состояний к метрикам
6. Decomposable
7. Multi-edges
8.  Ссылки на переиспользуемые элементы
9.  Import моделей
10. Вызов кодогенерации (скоро)