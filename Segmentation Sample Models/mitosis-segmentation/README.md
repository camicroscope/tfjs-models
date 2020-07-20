# Mitosis Segmentation
## Dataset 
The dataset used is available in [this](http://www.andrewjanowczyk.com/use-case-5-mitosis-detection/) post.

The dataset consist of 311 images of size 2,000 x 2,000 @*40x* selected from 12 breast cancer (BCa) patients. In total there are 550 mitosic centers expertly identified using a focal microscope.

This sample model is trained on br_masks for demonstration purpose to try to understand how to test models in caMicroscope.
## Preprocessing
Pixel values are normalized between 0-1.
## Model
U-net: 256 -> 128 -> 64 -> 32 -> 16 -> 32 -> 64 -> 128 -> 256.

Input image size: 256 x 256 x 3
