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

<div style={{ width: '100%', clear: 'both' }}>
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

<div style={{ width: '100%', clear: 'both' }}>
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

<div style={{ width: '100%', clear: 'both' }}>
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
Also you could add text label to the edge. To do that hover mouse on the edge and text field for the edge will appear
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./hoveredEdgeWithVisibleTextField.png 2x" alt="Hovered edge with a visible text field"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Just click on the text field in the same way as on the object and enter any text. Only a single line of text is allowed.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./edgeWithText.png 2x" alt="Edge with text"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
</div>

### Create a scheme with several objects and edges

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
You can continue add edges with object to build a chain. Just drag a new edge from the latest created object. The model size will be adjusted automaticaly.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./twoEdgesChain.png 2x" alt="Two edges chain"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Let update texts for object and edges labels
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./twoEdgesWithTextChain.png 2x" alt="Two edges chain"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Also you an drag an edge to an existing object. A new object will not be created in that case. Just hover edge on the existing object while dragging...
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./dragEdgeToExistingObject.png 2x" alt="Dragging edge to the existing object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
... and release it. The edge end position will be adjusted automaticaly.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./draggedEdgeToExistingObject.png 2x" alt="Dragged edge to the existing object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Let name the new edge.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./operationScheme.png 2x" alt="Opertation scheme"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
Well, we got a scheme of an operation, that consists of two transformation steps.
</div>

## Create a relation

We create the scheme of an operation above and intend, that the "operation" edge is equal to chain "transformation 1" -> "transformation 2". To emphasize that we can use Viete editor element relation. Relation shows, how an edge and a chain or two chains are related to each other.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To start creating relation click on the "operation" edge or its text field border with a left mouse button. The edge will be selected and become marked with red color.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./edgeSelection.png 2x" alt="Edge selection"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Select in the same way (with a left mouse button click) the first chain edge with label "transformation 1". The control to create relation will appear immidiately. Relation could be directional in one of two directions or bi-directional. So the control contains three buttons for that options.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./chainEdgeSelected.png 2x" alt="Chain edge selection"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Select the second chain edge with label "transformation 2". The control position will be updated.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./chainSelected.png 2x" alt="Chain selection"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Now let's create a bidirectional relation for a "operation" edge and the selected chain. Press the button with ⇔ sign. The relation will be created. There is a text field in relation, that allows to name it.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newRelation.png 2x" alt="New relation"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
Relations will not be used directly in that tutorial (but will do undirectly). The explanation for directional relations will be given in other pages of the documentation.
</div>

## Elements movement and navigation

The relation element created above overlaps with "operation" edge label. Let's see, how we can move elements to make everything visible clearly.

### Object movement

To move object drag it with mouse with **left mouse button** and **Shift** key holded.

### Edge label movement

You can also change edge label position which is influence on whole edge geometry. To move label drag it in the same way as object with mouse with **left mouse button** and **Shift** key holded.

### Move mode

Viete editor allows to switch into Move mode, when elements movement is possible without holding **Shift** key. That simplify elements movement, but edge dragging will not be possible in that mode.

Defualt mode for editor is Drag Edge mode. To switch into Move mode use Drag Edge button <img srcset="./dragEdgeModeButton.png 2x" alt="Drag Edge mode button"/> on the tool panel in the right. The editor mode will be switched into Move mode. And the button will be changed to Mode button <img srcset="./moveModeButton.png 2x" alt="Move mode button"/> to reflect that.

### Relation position

Relation position could not be changed directly. It is evaluated based on edges label position to be in the middle between edge chains.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
For our example relation we could move object and "operaton" edge lable to expand scheme a little so, that it will hold relation without significant overlapping.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./expandedSchemeToAvoidOverlapping.png 2x" alt="Expanded scheme without significant overlapping between relation and other elements"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
</div>

### Navigation

To move whole editor plane drag it at any point with **right mouse button** holded.

<!-- 1. Tuple для описания состояний
1. Choice для описания альтернатив в сценариях
2. Атрибуты для описания параметров действий
3. Mapping для декларации переходов от состояний к метрикам
4. Decomposable
5. Multi-edges
6.  Ссылки на переиспользуемые элементы
7.  Import моделей
8.  Вызов кодогенерации (скоро) -->