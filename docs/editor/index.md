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

To start draw a schema create a new project. Press button "Create project" a the top of the header
<img srcset="./createProject.png 2x" alt="Create project"/>

You will get an empty project. To draw anything in it add a model.

## Create model

To create a model open a context menu with a right mouse button click on any empty space and select menu item "Add model"

<img srcset="./addModel.png 2x" alt="Add model"/>

The new model will be created

<img srcset="./newModel.png 2x" alt="New model"/>


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