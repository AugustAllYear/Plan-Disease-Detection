<h1>
  <span class="prefix"></span>
  <span class="headline">Deep Learning Project: PyTorch or Keras</span>
</h1>

## About
For this project, you will design, train, and evaluate a deep learning model to solve a real-world problem of your choice. You will:
1. Select a data set that aligns with one of the themes from the course (image classification, text classification, or transfer learning).
2. Preprocess the data set to make it suitable for training a deep learning model.
3. Design and implement an appropriate architecture (CNN, RNN, or transfer learning).
4. Train and optimize your model using techniques learned in class.
5. Evaluate the model’s performance and document your findings.

You will also present your project to the class.

**Note:** We are including a predefined project option if you are uncertain where to start, see the [`project-plants`](./project-plants/) directory.

---

## Prerequisites
- Understand how neural networks work
- Run a neural network using PyTorch or Keras

---

## Deliverables

Materials must be submitted by the date provided by your instructor.

Your technical report will be hosted on GitHub Enterprise. Make sure it includes:

1. A **README.md** (that isn't this file) summarizing:
   - Problem statement and data set.
   - Model architecture and training process.
   - Results and key takeaways.
2. **Jupyter notebook(s)**: Include all code, visualizations, and explanations.  It does not have to be in just one notebook.
3. **Data set link**: Provide a link to your chosen data set.
4. Presentation slides for presenting your project to the class.
5. Any other necessary files (images, etc.)

**Submit your repo via google classroom.**

---

## Project Guidelines

### Data Set Selection
- Choose a data set from a publicly available source (e.g., [Kaggle](https://www.kaggle.com/discussions/general/199837), [UCI](https://archive.ics.uci.edu/datasets), or [TensorFlow Datasets](https://www.tensorflow.org/datasets)).
- The data set should have at least **1,000 samples** and include at least **three classes** for classification tasks.
- Ensure that the data set requires meaningful preprocessing (e.g., text tokenization, resizing images, or data augmentation).

### Example Data Sets

Need inspiration?  Here are some data sets you could use:
- **Images**: [CIFAR-100](https://www.cs.toronto.edu/~kriz/cifar.html), [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist)
- **Text**: [20 Newsgroups](http://qwone.com/~jason/20Newsgroups/), [IMDb Reviews](https://www.tensorflow.org/datasets/catalog/imdb_reviews)
- **Transfer Learning**: [Flowers Recognition](https://www.kaggle.com/alxmamaev/flowers-recognition)


### Project Phases

1. **Data Set Exploration and Preprocessing**
   - Define a clear problem statment for your project.
   - Describe the data set and its relevance to your project.
   - Visualize the data set (e.g., sample images, class distribution).
   - Preprocess the data to prepare it for training (e.g., normalization, tokenization, augmentation).

2. **Model Design and Implementation**
   - Choose an appropriate architecture:
     - **CNNs** for image data.
     - **RNNs** for sequential data.
     - **Transfer Learning** for pre-trained models.
   - Implement the architecture in PyTorch or Keras, documenting your decisions (e.g., choice of layers, activation functions).

3. **Training and Optimization**
   - Train the model on the data set, using an appropriate optimizer and loss function.
   - Experiment with techniques like learning rate tuning, dropout, and different optimizers.

4. **Evaluation**
   - Evaluate your model’s performance on a validation or test set.
   - Use appropriate metrics such as accuracy, precision/recall, or F1 score, depending on the task.
   - Visualize results (e.g., confusion matrix, loss/accuracy plots).

5. **Reflection and Documentation**
   - Summarize the strengths and weaknesses of your model.
   - Discuss potential improvements and additional experiments you would try with more time.

6. **Presentation**
   - **Must be within a time limit of 8 minutes.**
   - Use Google Slides or some other visual aid (Keynote, Powerpoint, etc).
   - Consider the audience.
   - Start with the **data science problem**.
   - Use visuals that are appropriately scaled and interpretable.
   - Talk about your procedure/methodology (high level).
   - Talk about your primary findings.
   - Make sure you provide **clear recommendations** that follow logically from your analyses and narrative and answer your data science problem.

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

1. **Data Set Exploration and Preprocessing**
   - Is there a clear problem statement for the project?
   - Is it clear what the learner plans to do?
   - Is the data set diverse, challenging, and well-documented?
   - Are missing values imputed appropriately?
   - Are distributions examined and described?
   - Are outliers identified and addressed?
   - Are appropriate summary statistics provided?
   - Are steps taken during data cleaning and EDA framed appropriately?
   - Does the learner address whether or not they are likely to be able to answer their problem statement with the provided data given what they've discovered during EDA?
   - Are categorical variables one-hot encoded?
   - Have the data been scaled appropriately?
   - Does the learner apply feature selection?
   - Does the learner properly split and/or sample the data for validation/training purposes?

2. **Model Design and Implementation**
   - Is the model architecture appropriate and well-justified?
   - Does the learner explain how the model works and evaluate its performance successes/downfalls?
   - Does the learner document key modeling decisions that they ahve made, e.g. choice of layers and activation functions?

3. **Training and Optimization**
   - Is training thorough, with experimentation?
   - Is the model trained on the data set using an appropriate optimizer and loss function?
   - Does the learner experiment with techniques like learning rate tuning, dropout, and different optimizers?

4. **Evaluation**
   - Does the learner accurately identify the baseline score?
   - Does the learner evaluate their model’s performance on a validation or test set?
   - Does the learner select and use metrics relevant to the problem objective and appropriate to the task?
   - Does the learner visualize the results of modeling?
   - Does the learner interpret the results of their model for purposes of inference?

5. **Reflection and Documentation**
   - Does the learner summarize the strengths and weaknesses of their model?
   - Does the learner provide appropriate context to connect individual steps back to the overall project?
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
