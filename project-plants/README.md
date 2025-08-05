<h1>
  <span class="prefix"></span>
  <span class="headline">Deep Learning - Project: Building an Image Classifier for Detecting Plant Diseases using PyTorch</span>
</h1>

## About
You've been hired as a data scientist for an agriculture tech company.  The company aims to help farmers identify diseases in their crops early on, to reduce losses and improve crop yields. 

Your task is to build an image classification model to detect plant diseases from leaf images.

Your model should classify images into multiple categories, such as healthy leaves or specific diseases (e.g., "Powdery Mildew," "Rust," "Leaf Spot"). This will help farmers take targeted action to treat their crops.

To accomplish this, you'll use a publicly available dataset of plant leaf images, the PlantVillage dataset, and PyTorch for building the classification model.

For this project, you will train and evaluate a deep learning model to solve a real-world problem. You will:
1. Set Up Your Notebook using Colab (recommended) or on your local machine
2. Preprocess and Transform the Data
3. Initialise (Build) the Model
4. Train the Model
5. Evaluate the Model
6. Conclusions and Recommendations

You will also present your project to the class.

We give you a starter notebook that provides a guided walkthrough of what you need to do, but if you want more of a challenge you can also ignore the starter code and write everything from scratch! 

---

## Project Guidelines

### Project Phases
Here is a suggested set of steps to follow:

1. **Set Up Your Notebook** Import the libraries you'll need and get the data set from [Kaggle](https://www.kaggle.com/datasets/mohitsingh1804/plantvillage). It's already split into training and validation sets.

2. **Data Preprocessing and Transformation:**
    - Resize the image size to 224x224 pixels.
    - Normalize the image data.
    - Apply data augmentations like random rotations or flips to improve generalization.

3. **Initialise (Build) the Model:** Use a pre-trained model (e.g., **ResNet18**) from `torchvision.models` and fine-tune it for the plant disease classification task.

4. **Train the Model:** Train the model on the training data set.
Use a suitable loss function (e.g., cross-entropy) and optimizer (e.g., Adam).

5. **Evaluate the Model:** Evaluate the model on the validation set. Report the overall model accuracy.

6. **Conclusions and Recommendations:** Is your model performance good enough for deployment in the real world? Is your model suitable for detecting some diseases but not others?

7. **Presentation**
   - **Must be within a time limit of 8 minutes.**
   - Use Google Slides or some other visual aid (Keynote, Powerpoint, etc).
   - Consider the audience.
   - Start with the **data science problem**.
   - Use visuals that are appropriately scaled and interpretable.
   - Talk about your procedure/methodology (high level).
   - Talk about your primary results.
   - Make sure you provide **clear recommendations** that follow logically from your analyses and narrative.

   Be sure to rehearse and time your presentation before class.

---

## Rubric

We will evaluate your project (for the most part) using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.

**Scores will be out of 27 points based on the 9 items in the rubric.** 
*3 points per section*

| Score | Interpretation |
| --- | --- |
| **0** | *Project fails to meet the minimum requirements for this item.* |
| **1** | *Project meets the minimum requirements for this item, but falls significantly short of portfolio-ready expectations.* |
| **2** | *Project exceeds the minimum requirements for this item, but falls short of portfolio-ready expectations.* |
| **3** | *Project meets or exceeds portfolio-ready expectations; demonstrates a thorough understanding of every outlined consideration.* |

### The Project Process

1. **Data Preprocessing and Transformation**
   - Is there a clear problem statement for the project?
   - Are the images resized?
   - Is the image data normalized?
   - Are data augmentations like random rotations or flips applied to improve generalization?
   - Does the learner properly split and/or sample the data for validation/training purposes?

2. **Initialise (Build) the Model**
   - Is the model architecture appropriate and well-justified?
   - Does the learner explain how the model works and evaluate its performance successes/downfalls?
   - Does the learner document key modeling decisions that they have made, e.g. choice of layers and activation functions?

3. **Train the Model**
   - Is training thorough, with experimentation?
   - Is the model trained on the data set using an appropriate optimizer and loss function?
   - Does the learner experiment with techniques like learning rate tuning, dropout, and different optimizers?

4. **Evaluate the Model**
   - Does the learner accurately identify the baseline score?
   - Does the learner evaluate their model’s performance on a validation set?
   - Does the learner select and use metrics relevant to the problem objective and appropriate to the task?
   - Does the learner interpret the results of their model for purposes of inference?

5. **Conclusions and Recommendations**
   - Does the learner summarize the strengths and weaknesses of their model?
   - Is it clear how the final recommendations were reached?
   - Are the conclusions/recommendations clearly stated?
   - Does the conclusion answer the original problem statement?
   - Does the learner discuss potential improvements and additional experiments they would try if they had more time?

6. **Presentation**
   - Is the problem statement clearly presented?
   - Does a strong narrative run through the presentation building toward a final conclusion?
   - Are the conclusions/recommendations clearly stated?
   - Is the level of technicality appropriate for the intended audience?
   - Is the learner substantially over or under time?
   - Does the learner appropriately pace their presentation?
   - Does the learner deliver their message with clarity and volume?
   - Are appropriate visualizations generated for the intended audience?
   - Are visualizations necessary and useful for supporting conclusions/explaining findings?


### Organization and Professionalism

**Project Organization**
- Are modules imported correctly (using appropriate aliases)?
- Are data imported/saved using relative paths?
- Does the README provide a good executive summary of the project?
- Is markdown formatting used appropriately to structure notebooks?
- Are there an appropriate amount of comments to support the code?
- Are files & directories organized correctly?
- Are there unnecessary files included?
- Do files and directories have well-structured, appropriate, consistent names?

**Visualizations**
- Are sufficient visualizations provided?
- Do plots accurately demonstrate valid relationships?
- Are plots labeled properly?
- Are plots interpreted appropriately?
- Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report?

**Python Syntax and Control Flow**
- Is care taken to write human readable code?
- Is the code syntactically correct (no runtime errors)?
- Does the code generate desired results (logically correct)?
- Are libraries used appropriately?


In order to pass the project, learners must earn a minimum score of 1 for each category.
- Earning below a 1 in one or more of the above categories would result in a failing project.
- While a minimum of 1 in each category is the required threshold for graduation, learners should aim to earn at least an average of 1.5 across each category. An average score below 1.5, while it may be passing, means learners may want to solicit specific feedback in order to significantly improve the project before showcasing it as part of a portfolio or the job search.

### REMEMBER:

This is a learning environment and you are encouraged to try new things, even if they don't work out as well as you planned! While this rubric outlines what we look for in a _good_ project, it is up to you to go above and beyond to create a _great_ project. **Learn from your failures and you'll be prepared to succeed in the workforce**.

---
