# Visualise models as object diagrams with Picto

This repository includes a project with two Picto visualisations:

- An Ecore visualisation that shows the contents of a metamodel using a class diagram notation.
- A model visualisation that shows the contents of a model using an object diagram notation.

Both visualisations use [PlantUML](https://plantuml.com/) as the graphical notation to visualise the models, and they originate from the [Epsilon Playground](https://eclipse.dev/epsilon/playground/). The model-to-text transformations that generate the views are present in the `picto` folder of the `picto.plantuml.objectdiagram` Eclipse project. These are single-view Picto visualisations, so no tree to select different views is generated.

## How to use the visualisations

1. Download the repository to your machine and import the Eclipse project into your workspace.
2. The project contains, apart from the `picto` folder that contains the visualisations, an example model and meta-model extracted from Picto's Social Network example.
3. Register the `socialnetwork.ecore` metamodel. Right click > *Register EPackages*.
4. Open the `socialnetwork.model` file. Once the XMI tree editor opens, you can also open the `Picto` view to see the object diagram visualisation.
5. You can also open the `socialnetwork.ecore` model and see how Picto then shows the metamodel contents using a class diagram.

## How to visualise my models with the Picto visualisations

1. Copy the `picto` folder to the Eclipse project you are working in.
2. Besides the `.ecore` or `.model` file that you want to visualise, you must create a file with the same name plus the `.picto` extension. If you look at the provided project, there is a `socialnetwork.model.picto` file that accompanies the `socialnetwork.model` file.
3. Copy the contents of the `socialnetwork.model.picto` file (or the `socialnetwork.ecore.picto` file if you are visualising a metamodel) to the `.picto` file that you have created.
4. Adapt the `transformation` path in the `.picto` file based on the location of the file and the `picto` folder.
5. If everything went well, now you should be able to see your model visualised in the Picto window.

## Extra information

- [Picto documentation](https://eclipse.dev/epsilon/doc/picto/)
- [Extra picto articles](https://eclipse.dev/epsilon/doc/articles/#picto)
