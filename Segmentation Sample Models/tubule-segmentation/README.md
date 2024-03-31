# Tubule Segmentation
## Dataset 
The dataset used is available [here](http://andrewjanowczyk.com/wp-static/tubule.tgz) .

The dataset consist of 85 images ColoRectal images scanned at 40x., where each image is 775 x 522 and contains a total of 795 regions.  The tubules were manually annotated across all images by an expert pathologist.

This sample model is trained on br_masks for demonstration purpose to try to understand how to test models in caMicroscope.
## Preprocessing
Patch Extraction is performed.
Pixel values are normalized between 0-1.
## Model
U-net: 256 -> 128 -> 64 -> 32 -> 16 -> 32 -> 64 -> 128 -> 256.

Input image size: 256 x 256 x 3

