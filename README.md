# caMicroscope-tfjs-models
Sample models for caMicroscope

## Common Issues:
- ***Provided weight data has no target variable***: This might be a common issue for the model to fail to load. To avoid this, make sure that the keras model is loaded exactly once. To make sure, reset the runtime and load the model before carrying to conversion. This case also goes when your converting using the bash command. The Keras model which you saved must be loaded just once. To make sure, save the model, reset the runtime, load the model and save it again. Multiple loads seem to mess up the layer names. You can track this issue further [here](https://github.com/tensorflow/tfjs/issues/755).
