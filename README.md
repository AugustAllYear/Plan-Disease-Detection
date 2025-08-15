<h1>
  <span class="prefix"></span>
  <span class="headline">Plant Disease Detection</span>
</h1>

## Problem Statement

Can plant disease be identified by a Convolutional Neural Network model trained on images to aid farmers in preventing the loss of crops?
The simplest approach will be to develop an image classification model broken into categories of known diseases to train the model on. This is to aid the farmer in knowing what treatment will best prevent the loss of each specific type of crop.
The baseline for training will be images of healthy plants, though the Neural Net will not be aware as it will organize images purely on similarity of features.

Further we could refine the model, collect more data to identify disease at early stages if the present model proves useful.

We will explore this question with the use of  a Pytorch Resnet 18 model.
Thanks to a great dataset we will be able to categorically sort the images for a more precise insight into the cause of the plant's disease state.


---


### Table of Contents

Problem Statement
- Table of Contents
- Data
Methodology
- Preprocessing
- Modeling
Results
- Key Findings
- Conclusion and Recommendations
Setup and Usage
Contributors
Additional Information


---


## Methodology

The following are the steps that were taken in the jupyter notebook named plant_disease_detection.

### Preprocessing
1. Obtain data:

    The [data set](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset/data.) was retreived from Kaggle.com.
    This dataset is pre sorted into a training and validation set and further sorted species per disease state/healthy.
    It contains over 50,000 images divided into 38 classes each containing approximtley 1,300 images per class for the model to train on.

2. Preprocess and transform the data:
 - Set image dimensions to 224x224 pixels.
 - Apply random horizontal flip with 50% probability to improve generalization
 - Apply normalization to image data.
 - Transform to tensor

### Modeling

1. Build Model: [ResNet-18 (read more here)](https://docs.pytorch.org/vision/main/models/generated/torchvision.models.resnet18) with pre-trained ImageNet weights
    num_epochs = 10 - this was limited due to computing capacity/limited number of cpus
    batch_size = 32
    learning_rate = 0.001
    optimizer = optim.Adam(model.parameters(), lr=learning_rate)

   Applied CrossEntropy Loss Function to quantify difference of model's predicted probability distribution and the true distribution of the data. 
   
2. Train Model
  
3. Validation


---


## Results
### Key Findings: 
The Resnet 18 model achieved an accuracy score of 98.64% without iterating on parameters due to time constraints. By standard image classification practices in Data Science this is considered an excellent score, but that is in the world a data. It would be most useful to discuss with the farmers the risks involved in miss treating certain crops as it may too cause a loss though one would hope not as substantial as losses incurred from the disease state itself. 

### Conclusion and Recommendations
If upon the framers recommendation they would like to do some onsite/in the field testing and delay further model refinement for when we expand the models capacity for potential wider species familiarity the following recommendations order may be shuffled, but generally speaking we suggest the following:


1. Increase budget for GPU: this would allow tweaking of hyper parameters to try to get a score closer to 99.5 or so.
2. More photos of diseases at different stages for early detection
3. Diversify the number of species for identification.
4. Currently the model is classifying diseases by type on different Cultivars.
    - Work directly with the farmers to see if identifying disease by treatment type (aggregate multiple disease categories by types of treatments likely certain treatments work for multiple diseases) This would allow for simplification of the model in certain respects so it could expand its range in other ways without losing efficiency to enhance it elsewhere for example in range of identifiable species and their disease states.
5. Use GradCAM such as described in this [article](https://medium.com/@stepanulyanin/implementing-grad-cam-in-pytorch-ea0937c31e82) could prove extremely useful in understanding what types of images lead to miss classification or increase Accuracy of classification.
6. Develop an interface for farmers to be able to use the models and on site testing.
7. Develop a refined, clear and simple to implement mobile application and possible kit for image capture standardization to allow farmers to begin to capture images of diseased and healthy crops alike in the field. It could include a testing kit and specimen collection to be sent to a lab for testing with the complete image and specification folder so data sets for other regions could be compiled in real time.


---


## Setup and Usage

**Installation Instructions:**
- Clone this repository
- Install requirements with `pip install -r requirements.txt` (if available)

**Running the Code:**
- Open and run `Baseline_Model_Data.ipynb` (polling analysis)
- Open and run `youtube_scraper.ipynb` (data collection) and `processing_modeling_visualization.ipynb` (sentiment analysis)

**Example Usage:**
- See provided notebooks for usage examples and to reproduce all results
  
### Tech

Pretrained **ResNet18**) from `torchvision.models`

---

## Contributors

- **August vollbrecht** augustvollbrecht@gmail.com

-  **Special Thanks:**
1. Hank Butler
2. Alanna Besaw
3. General Assembly staff and instructors
  
### Credit and Sources (vis-a-vis technical requirements)

**Technical Support:**

- Jupyter Labs
- Colab
- Python

Libraries:

jupyter                   (1.1.1)
jupyter_client            (8.6.3)
jupyter-console           (6.6.3)
jupyter_core              (5.7.2)
jupyter-events            (0.12.0)
jupyter-lsp               (2.2.5)
jupyter_server            (2.15.0)
jupyter_server_terminals  (0.5.3)
jupyterlab                (4.4.0)
jupyterlab_pygments       (0.3.0)
jupyterlab_server         (2.27.3)
jupyterlab_widgets        (3.0.14)
pandas                    (2.2.3)
python                    (3.13.2)
Pytorch Venvs:
activate
activate.csh
activate.fish
Activate.ps1
debugpy
debugpy-adapter
f2py
fonttools
hf
httpx
huggingface-cli
ipython
ipython3
isympy
jlpm
jsonpointer
jsonschema
jupyter
jupyter-console
jupyter-dejavu
jupyter-events
jupyter-execute
jupyter-kernel
jupyter-kernelspec
jupyter-lab
jupyter-labextension
jupyter-labhub
jupyter-migrate
jupyter-nbconvert
jupyter-notebook
jupyter-run
jupyter-server
jupyter-troubleshoot
jupyter-trust
kaggle
normalizer
numpy-config
pip
pip3
pip3.13
pybabel
pyftmerge
pyftsubset
pygmentize
pyjson5
python
python3
python3.13
send2trash
slugify
tiny-agents
torchfrtrace
torchrun
tqdm
transformers
transformers-cli
ttx
wsdump


- imports:
import kagglehub
<!-- import matplotlib.pyplot as plt optional for further modeling -->
import numpy as np
import os
import pandas as pd
import torch
import torch.nn as nn
import torch.optim as optim
import torchvision
import torch.nn.functional as F
import torchvision.transforms as transforms
<!-- import seaborn as sns optional for further modeling  -->

from sklearn.metrics import confusion_matrix
from sklearn.metrics import classification_report
from torchvision.datasets import ImageFolder
from torch.utils.data import DataLoader, Dataset
from torchvision import datasets, transforms, models

   
---


## Additional Information

Please reachout to: augustvollbrecht@gmail.com with any questios or sugestions!

**Licensing:** MIT License 


---
