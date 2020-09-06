# Understanding our interface

Below is an introduction to the AlphaHub platform's interface. We recommend you to [login](https://www.alphahub.dev/login) on AlphaHub and follow this introduction step-by-step to fully understand all parts of the platform.

---

# Project listing page
The first page after you login on AlphaHub.

![](assets/images/interface/landing.png)

You can click on **Create new project** to start a new project or **Go to project** to continue an existing project. You can remove or duplicate any project using the options on the top-right of the project tile.

---

# Contextual Search

![](assets/images/interface/create.png)

Once you click on **Create new project**, you will be asked to provide a name for your project and a search query. The search field is what we call contextual search, and it is meant to understand your problem statement in plain English.

For example, if you want to make a model which detects faces then you can type `Identify different faces` in the search query. We have created a recommendation engine that will understand your search query and provide step-by-step assistance when you start developing your model.

---

# Canvas

![](assets/images/interface/canvas.png)

When you start a new project or open an existing project, you are presented with the above canvas. In the left panel you have PyTorch layers and on the right is the canvas where you will design your model.

`PyTorch layers are like lego pieces, you connect them in different ways to create a model, also referred to as architecture.`

We also pre-select the first layer of your model using the contextual search feature or put a standard placeholder.

---

# Layers

The left panel on the canvas has all the PyTorch layers grouped by categories. You can click and expand any category to select a particular layer and then drag-and-drop it on the canvas. If you click on the settings icon on the top-right of any layer in the canvas, a panel will appear from the right side.

![](assets/images/interface/layer.png)

This panel has two parts:

  *  The first part is the **recommendation engine** that we discussed earlier with the contextual search. It provides you with top-3 recommendations for the next possible layer based on your current model structure and your search query. We are making sure that you don’t have to waste time figuring out which layer to add either as a beginner or a researcher.

  * The second part is the parameters panel, these are the parameters that are required by the layer to function properly. Parameters with a red asterisk are required parameters and the remaining are optional parameters.

---

# Model

As we mentioned earlier, creating a model is like making a structure using lego pieces and our lego pieces are the PyTorch layers. There are 2 ways to add layers to the model, first is by finding it on the left panel and dragging it on the canvas. Second is using our recommendation engine and clicking on `Add to model`. This will add the layer on the canvas.

`Adding layers on the canvas is the first step, you have to connect all the layers yourself. We are working on our engine to show suggested connections to different layers on the canvas.`

![](assets/images/interface/model.png)

Here are some points to keep in mind when you design your model:

* Once you add a layer, you can connect any two layers by dragging a connector from **Out to In**. 
* You are free to move around your layers, the **connectors are fluid**. 
* There is an **x** button on the top-right of the layer which will **delete the layer**.
* If you want to delete a connection, press `Shift+click` on the connection and then press the Delete key. Just clicking on connections will add clip points.
* Layers can have multiple outward connectors and multiple inward connectors. **You are not constrained to sequential structures**.

---

# Visual IntelliSense

![](assets/images/interface/intellisense.png)

We understand that model development is hard and you worry about the tensor errors - the most time-consuming part of model development.

## Development without AlphaHub

* Usually, after defining a model, you have to run the model to find errors and then debug the code to figure out where exactly is the problem.
* Then you search that area of the code on StackOverflow to find a potential solution.
* Then you fix that part of the code and repeat the running-debugging cycle, which can take from hours to weeks depending upon experience and expertise.

## Development With AlphaHub

* Define a model on the canvas and click **Save draft**.
* We save the model state for you and execute the running-debugging cycle for you.
* We find the error in your graph and pinpoint its location.
* We analyze the error and find its solution, and present it to you in a subtle way.
* All of that happens in real-time, in a second!

---

# Complex Models

![](assets/images/interface/model.png)

We agree that it looks a bit ugly but remember, the connections are fluid! You can make it look however you want, and we preserve that structure for you because we know that different people find meaning in different structures.

