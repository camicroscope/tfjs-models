## Details
The image dataset is composed of high-resolution (2040 × 1536 pixels), uncompressed, and annotated H&E stain images from the Bioimaging 2015 breast histology classification challenge [3]. All the images are digitized with the same acquisition conditions, with magnification of 200× and pixel size of 0.42μm × 0.42μm. Each image is labeled with one of four classes: i) normal tissue, ii) benign lesion, iii) in situ carcinoma and iv) invasive carcinoma

Input size = 512 x 512 x 3

## Citation
In this notebook, there's a Keras implementation of the patch-wise network of the paper <a href="https://arxiv.org/abs/1803.04054">Two-Stage Convolutional Neural Network for Breast Cancer Histology Image Classification</a>:

```
@inproceedings{nazeri2018two,
  title={Two-Stage Convolutional Neural Network for Breast Cancer Histology Image Classification},
  author={Nazeri, Kamyar and Aminpour, Azad and Ebrahimi, Mehran},
  booktitle={International Conference Image Analysis and Recognition},
  pages={717--726},
  year={2018},
  organization={Springer}
}
```
