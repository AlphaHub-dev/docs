# Terminologies

Allow us to introduce some terminologies that will help you navigate and build faster with AlphaHub.

---

## Layer panel and Canvas

Once you create or resume a project, you are greeted with this window. The panel on the left is the layer panel and the larger area on the right is the Canvas.

![](assets/images/terminologies/canvas.png)

### Layer Panel

The layer panel consists of three sections, namely, layers, blocks and models.

  1. **Layers**: These are the building blocks for models. You can think of them as Lego pieces that you can use in different layouts and create a model.
  2. **Blocks**: Some layers can be grouped together in a particular layout and re-used in different parts of the model. These groups are called blocks, and you will hear about Basic-Block, Bottleneck-Block, Transformer-Block as you dive deeper into AI modelling.
  3. **Models**: You create models using layers and blocks but, sometimes you want to use existing models that are designed and trained by researchers. These models provide out-of-the-box performance, and using them as a sub-part of your model is called transfer learning. More on types of models later.

### Canvas

The area where you design a model by adding layers, blocks or models. You can connect anything in the canvas using the IN and OUT connectors. You can also zoom in/out in the canvas to view larger models.


## Parameter panel

If you click on the settings icon on the top-right of any layer, you will have access to the parameter panel.

![](assets/images/terminologies/sidebar.png)

`This panel is used to define the configuration of a layer. These layer parameters play a crucial role in processing the data that you use to train your model.`

There are two sub-parts of this panel, the top is the recommendation section and the bottom is the parameters section.

  1.  **Recommendation**: We use your inputs from the contextual search to find out which layer is important for your model. We simultaneously analyse the state of your model and suggest the top-3 layers for your model.

  2.  **Parameters**: Here you provide the configuration for the layer. Required parameters are marked with a red asterisk and remaining parameters are optional. In case you are not sure about the parameters, you can enter random numbers and the Visual Intellisense component of the platform will assist you.

## Model

A model is a collection of layers or blocks in a particular layout. This layout is also referred to as the architecture of the model. Below is an example of the ResNet18 model.

![](assets/images/terminologies/resnet18.png)

Once the architecture is designed, you can train your model and share it. There are many publicly available models that are used to jump-start the training process. These pre-trained models are tweaked and fine-tuned for a particular use-case.

  1.  **Pre-trained**: Most AI libraries provide a number of pre-trained models; we will add these models in the layer panel under the Models tab in the upcoming release. You can easily drag-and-drag these models like you would with a layer or a block.

  2.  **AlphaHub pre-trained**: AlphaHub allows defining models as graphs, we will provide all standard models as graphs that you can add to your projects. If you want to tweak any part of a pre-trained model, you can expand the model in a different view in the canvas, make the changes and come back to the original project. This allows you to alter any pre-trained model at a more granular level without leaving the canvas.