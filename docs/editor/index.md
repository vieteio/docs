---
sidebar_position: 2
---
# Editor tutorial

This tutorial demonstrates how to use an editor for a DAO economic model modeling task as an example.

In the context of the DAO modeling task, the editor enables:
1. To describe the general schema of DAO mechanics in a free form.

<img src="./useCaseAndGovernance.png" alt="DAO general schema" width="400"/>

2. To describe the evaluation logic for metrics (for example, token price) in a decomposable manner.

<img src="./metricEvaluation.png" alt="Metirc evaluation" width="400"/>

3. To generate Python code for probabilistic modeling, which will run the modeling and display plots for selected metrics as the result of the modeling.

 Consequently, we will depict the schemas of the Freelance DAO project, as illustrated by the fragments in the screenshots above.

## Create project

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To commence the process of creating a schema, you will need to create a new project. To do so, simply press the "Create Project" button located at the top of the header.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./createProject.png 2x" alt="Create project"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
This will result in the creation of an empty project. To add content to the project, you will need to add a model.
</div>

## Create model

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create a model, open the context menu by right-clicking on an empty space, and select the "Add Model" option from the menu.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addModel.png 2x" alt="Add model"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Upon selecting the "Add Model" option, a new model will be created.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newModel.png 2x" alt="New model"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
With the creation of the new model, you can now proceed to create objects and edges to draw your desired scheme.
</div>

## Create objects and edges

It is important to note that objects can only be created within a model, while edges can be drawn between any objects, regardless of whether they belong to the same model or different models. 

> Note: Additionally, it is allowed to draw an edge from an object into another edge, however, this cannot be done in reverse. We will discuss this in greater detail later on.

### Create object

<div style={{ width: '50%', float: 'left', clear: 'left' }}>

To create an object, right-click on any empty space *within the model* to open the model context menu and select the "Add Object" option.

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addObject.png 2x" alt="Add object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Upon selecting the "Add Object" option, a new object will be created within the model.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newObject.png 2x" alt="New object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
To label the object with text, such as the object's name, simply click on the object with the left mouse button. This will bring up the cursor, allowing you to enter text.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./cursorInsideObject.png 2x" alt="Cursor inside an object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Enter the desired text. Please note that only a single line of text is permitted.

To remove the cursor, simply click on any empty space within the editor or the model.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newObjectWithName.png 2x" alt="Object with a text inside"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
</div>

### Create edge

Viete is designed to facilitate the rapid creation of chains of objects connected by edges. As a result, the process of creating an edge has been optimized to require the minimum number of actions possible.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create an edge, simply click on an object with the left mouse button and drag the mouse away from the object. This will cause an edge to appear, originating from the object and extending to the mouse pointer.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./dragEdge.png 2x" alt="Dragging edge from an object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Once the mouse button is released, the edge will be created along with a new object at the end of the edge.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newObjectAndEdge.png 2x" alt="Created edge with a new object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
You can label the new object with text as previously described.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newNamedObjectAndEdge.png 2x" alt="Created edge with a named end object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
You may also add a text label to the edge by hovering your mouse over the edge, which will bring up the text field for the edge.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./hoveredEdgeWithVisibleTextField.png 2x" alt="Hovered edge with a visible text field"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Simply click on the text field in the same manner as you would with an object, and enter the desired text. 
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./edgeWithText.png 2x" alt="Edge with text"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
</div>

### Create a scheme with several objects and edges

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To build a chain, you may continue to add edges with objects by dragging a new edge from the previously created object. The size of the model will automatically adjust to accommodate the added elements.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./twoEdgesChain.png 2x" alt="Two edges chain"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
You can revise and update the texts for the object and edge labels.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./twoEdgesWithTextChain.png 2x" alt="Two edges chain"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Additionally, you can also drag an edge to an existing object. In that case, a new object will not be created. Simply hover the edge over the existing object while dragging …
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./dragEdgeToExistingObject.png 2x" alt="Dragging edge to the existing object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
... and then release the mouse button. The endpoint of the edge will be automatically adjusted.
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
We have now created a scheme of an operation that consists of two transformation steps.
</div>

## Create a relation

We created the schema of the operation above, with the intention that the "operation" edge represents the chain "transformation 1" -> "transformation 2". To emphasize this, we can use the Viete editor element relation. The relation displays the relationship between an edge and a chain or two chains.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create the relation, click on the "operation" edge or its label border with the left mouse button. The edge will be selected and highlighted in red to indicate it is selected.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./edgeSelection.png 2x" alt="Edge selection"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Then select the first chain edge labeled "transformation 1" in the same manner. The control to create the relation will become available. The relation can be unidirectional or bidirectional, and the control provides three buttons to choose from.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./chainEdgeSelected.png 2x" alt="Chain edge selection"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Then, select the "transformation 2" edge in the same manner and the control will be updated.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./chainSelected.png 2x" alt="Chain selection"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
To create a bidirectional relation between the "operation" edge and the selected chain, click on the button with the ⇔ symbol in the control. The relation will be established, and a text field will become available for naming the relation.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newRelation.png 2x" alt="New relation"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
Further explanations regarding directional relations will be provided in other sections of the documentation.
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

## Create tuple

Let's move on to creating the Freelance DAO schema. We already used edges to represent operation or transformation, while objects represented states. In real tasks state could be compound, i.e. consisting of several parameters. Tuple allows to represent such state.

In out DAO a client with a task will be able to register the task in the DAO. Let's create a tuple to represent pair of a client and a task.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>

To create a tuple open a model context menu with a right mouse button click on any empty space *inside the model* and select menu item "Add tuple"

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addTuple.png 2x" alt="Add tuple"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>

The new tuple with zero components will be created inside the model.

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newTuple.png 2x" alt="New tuple"/>
</div>

<div style={{ width: '100%', clear: 'both' }}>
</div>

### Add a component to the tuple

<div style={{ width: '50%', float: 'left', clear: 'left' }}>

Plus sign **+** button allows to add components to the tuple. Press the button twice to add two components. Every component of a tuple is an independent object.

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./tupleWithTwoComponents.png 2x" alt="Tuple with two components"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>

You can set text in component in the same way, as for object. Let's name the components as 'client' and 'task'.

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./tupleWithTwoNamedComponents.png 2x" alt="Tuple with two components"/>
</div>

<div style={{ clear: 'both' }}>
</div>

### Drag edge from tuple

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
We need to describe an operation of publishing the task on a blockchain. To do that we should drag from a tuple an edge with a new object, that will respresent the state of a registered task.

An edge can be dragged from a component or from the tuple itself. To drag an edge from the tuple hover a mouse on a tuple, but not on any of its components, and start dragging edge.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./dragEdgeFromTuple.png 2x" alt="Drag edge from tuple"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
The new edge and object will be created. We can name the edge with a label "publish on DAO".
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./edgeFromTuple.png 2x" alt="Edge dragged from tuple"/>
</div>

<div style={{ clear: 'both' }}>
</div>

### Convert to tuple

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
Let's turn the new object into tuple to describe the state of a published task more precise. To do that open the object context menu with a right mouse button click and choose "Convert to tuple" option.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./convertToTuple.png 2x" alt="Convert to tuple"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
The object will be replaced with a tuple with one component. Note, that the edge will be targeted to the created tuple, not it's component.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./convertedToTuple.png 2x" alt="Tuple converted from object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Add the second component and name the components. In the DAO client is represented by it's accound, and task has status of published.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./publishedTask.png 2x" alt="Published task"/>
</div>

<div style={{ clear: 'both' }}>
</div>

### Describe an object properties with a tuple

Notice, how we made a transition from some not formalized but quite clear entities "client" and "task" to formalized "client's account" and "published task". The last entities could be described precisely. We touch briefly how to do that in this tutorial and deeper in other pages of the documentation.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>

Let's describe "published task". Published task in a Freelance DAO should have a description and a budget for execution. To describe that drag a tuple with two components from a "published task" component, i.e. drag and object, convert it into a tuple and add the second component.

More advanced is to set a string type to "description" and number type to "budget". That details are out of scope of this tutorial.

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./componentProperties.png 2x" alt="Published task properties"/>
</div>

<div style={{ clear: 'both' }}>
</div>

## Create choice

Let's describe another Freelance DAO usecase. A worker for the task is found and necessary price for the task execution is locked in the blockchain. Task execution could proceed in a two ways. First way is the task is executed well and accepted by the client. Another way is the task is not accepted by the client by some cause. To describe such alternative Viete editor offers choice element.

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
You could create an empty choice element from model context menu with "Add choice" option.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addChoice.png 2x" alt="Add a choice"/>
</div>

<div style={{ clear: 'both' }}>
For our case it will be more convinient to create a choice in another way.
</div>

### Convert to choice

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
We have initially a tuple with worker's account, task and locked price. Edge with label "execution" should start from the tuple and end in choice element.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./initialTaskExecutionTuple.png 2x" alt="Tuple with task execution conditions"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'left' }}>
To create the edge we firstly drag from the tuple an edge with a new object...
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./dragExecutionEdge.png 2x" alt="Drag execution edge with a new object"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
... and then open the object context menu and choose "Convert to choice" option.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./convertToChoice.png 2x" alt="Convert to choice option in menu"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
We will get a choice with the only one component.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./convertedToChoice.png 2x" alt="Object converted to choice"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>

Let's add the second one with **+** button and name the components.

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./choiceWithAlternative.png 2x" alt="Choice with execution result alternative"/>
</div>

<div style={{ clear: 'both' }}>
</div>

### Use case with several choices

Let's continue to describe use case with task execution.

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
If the work is accepted, the worker should get a reward.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./workerReward.png 2x" alt="Worker reward"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Otherwise the client should get his payment back or the worker can disagree and open a dispute. The judge will solve the dispute and choose one of two possible alternatives.

Scheme for that logic with several branching will have several choices.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./judgment.png 2x" alt="Judgment for work acception/rejection"/>
</div>

<div style={{ clear: 'both' }}>
</div>

## Edge attribute

Usecase above has two actors: client and worker. Judgment process assumes, that there is one more actor - a judge (or may be several judges). To put judge into scheme without remakin schemen significantly we could add him/her as an attribute for edge "judment".

Edge attribute is an object with an edge going from the object to attributed edge. It could be added manually by creating the object and the edge. But Viete editor offers automation for that.

<div style={{ width: '50%', float: 'left', clear: 'both' }}>

To add an attribute to the edge open the edge context menu with a right mouse button click on the edge or it's label and select menu item "Add attribute".

</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./addAttribute.png 2x" alt="Add attribute"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
An empty attribute will be created as an object linked (by an edge) to the edge label. Position for the attribute will be chppose automaticaly. You can move the attribute to any other position.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./newAttribute.png 2x" alt="New attribute"/>
</div>

<div style={{ width: '50%', float: 'left', clear: 'both' }}>
Also you can enter a name for the attribute.
</div>

<div style={{ width: '50%', float: 'right', clear: 'right' }}>
<img srcset="./namedAttribute.png 2x" alt="Named attribute"/>
</div>

<!--
1. Атрибуты для описания параметров действий
2. Mapping для декларации переходов от состояний к метрикам
3. Decomposable
4. Multi-edges
5. Ссылки на переиспользуемые элементы
6. Import моделей
7. Вызов кодогенерации (скоро) -->