# YNet
## Dataset 
The dataset used is available in [this](https://www.bcsc-research.org/data/variables/) post.
A total of 87 pathologists diagnosed a randomly assigned subset of 60 slides into four diagnostic categories (benign, atypia, ductal carcinomain situ, and invasive cancer),producing an average of 22 diagnostic labels per case.  The average size of these ROIs is10,000×12,000. We use these 200 ROIs for our data set.

## Model
[Y-net](https://arxiv.org/pdf/1806.01313.pdf): 


Input image size: 256 x 256 x 3


Citation 

``` @inproceedings{mehta2018ynet,
  title={{Y-Net: Joint Segmentation and Classification for Diagnosis of Breast Biopsy Images}},
  author={Sachin Mehta and Ezgi Mercan and Jamen Bartlett and Donald Weaver and Joann  Elmore and Linda Shapiro},
  booktitle={International Conference on Medical image computing and computer-assisted intervention},
  year={2018},
  organization={Springer}
}
```
