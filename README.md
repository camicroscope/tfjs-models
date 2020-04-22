<h2 align="center">
  <a href="http://camicroscope.org/"><img src="https://avatars2.githubusercontent.com/u/12075069?s=400&v=4" style="background-color:rgba(0,0,0,0);" height=230 alt="camicroscope: a web-based image viewer optimized for large bio-medical image data viewing"></a>
</h2>

# Sample models for caMicroscope.

## Classification Models
The following sample classification models can be used by caMicroscope's predict application as-is.
* [ICAR18](Classification%20Sample%20Models/ICIAR18_data_IRRCNN_model) -- [model](Classification%20Sample%20Models/ICIAR18_data_IRRCNN_model/tfjs_model/model.json) and [weights](Classification%20Sample%20Models/ICIAR18_data_IRRCNN_model/tfjs_model/group1-shard1of1.bin)
* [Bioimaging15](Classification%20Sample%20Models/classification-of-HnE-stained-histological-breast-cancer-images) -- [model](Classification%20Sample%20Models/classification-of-HnE-stained-histological-breast-cancer-images/tfjs_model/model.json), [weights part 1](Classification%20Sample%20Models/classification-of-HnE-stained-histological-breast-cancer-images/tfjs_model/group1-shard1of2), and [weights part 2](Classification%20Sample%20Models/classification-of-HnE-stained-histological-breast-cancer-images/tfjs_model/group1-shard2of2)
* [Lymphoma](Classification%20Sample%20Models/lymphoma-cancer-classification) -- [model](Classification%20Sample%20Models/lymphoma-cancer-classification/model/tfjs_model/model.json), and [weights](Classification%20Sample%20Models/lymphoma-cancer-classification/model/tfjs_model/group1-shard1of1)

## Segmentation Models
The following segmentation models can be used by caMicroscope's segmentation algorithm, as an alternative to traditional CV methods.
* [Mitosis](egmentation%20Sample%20Models/mitosis-segmentation) -- [model](Segmentation%20Sample%20Models/mitosis-segmentation/tfjs_model/model.json), [weights part 1](Segmentation%20Sample%20Models/mitosis-segmentation/tfjs_model/group1-shard1of2.bin), and [weights part 2](Segmentation%20Sample%20Models/mitosis-segmentation/tfjs_model/group1-shard2of2.bin). 

## Common Issues:
- ***Provided weight data has no target variable***: This might be a common issue for the model to fail to load. To avoid this, make sure that the keras model is loaded exactly once. To make sure, reset the runtime and load the model before carrying to conversion. This case also goes when your converting using the bash command. The Keras model which you saved must be loaded just once. To make sure, save the model, reset the runtime, load the model and save it again. Multiple loads seem to mess up the layer names. You can track this issue further [here](https://github.com/tensorflow/tfjs/issues/755).
- Don't use Keras' Lambda in model definition. If want to use, save weights, remove Lambda calls, load weights again and then save the complete model as .hdf5

## Contributing
Feel free to contribute:).
