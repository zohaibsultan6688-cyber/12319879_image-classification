
# 12319879_image-classification

**Author:** Zohaib Sultan  
**Course:** Applied Deep Learning  
**Assignment:** Assignment 1 - Initiate

## 1. Project Overview

**Project Title:** Image Classification on CIFAR-10 Using a Custom CNN
and Transfer Learning  
This project focuses on image classification using deep learning. The
objective is to build a baseline Convolutional Neural Network (CNN) from
scratch and compare it with a pretrained ResNet-18 model fine-tuned on
the CIFAR-10 dataset.

### Research Questions

1.  How does a custom CNN compare with a pretrained ResNet-18 on
    CIFAR-10?
2.  How do data augmentation and hyperparameter tuning affect
    classification performance?
3.  What trade-offs exist between classification performance and
    training time?

### Proposed Approach

1.  **Baseline Model:** Build and train a lightweight custom CNN from
    scratch.
2.  **Transfer Learning:** Use an ImageNet-pretrained ResNet-18 and
    adapt its final classification layer for the 10 CIFAR-10 classes.
3.  **Data Augmentation:** Apply random horizontal flipping and small
    rotations during training. Evaluate color jitter as an optional
    experiment.
4.  **Optimization:** Experiment with learning rates, batch sizes,
    optimizers, and learning-rate scheduling.
5.  **Evaluation:** Compare models using accuracy, macro-precision,
    macro-recall, macro-F1 score, confusion matrices, and training time.
6.  **Application:** Develop an interactive image-classification demo
    using Streamlit or Gradio.

------------------------------------------------------------------------

## 2. Selected Project Type

- **Type:** Bring Your Own Method \[cite: 3\]
- **Description:** This project uses a publicly available benchmark
  dataset \[cite: 3\] and implements and compares deep-learning methods.
  A custom CNN will establish a baseline, while ResNet-18 will provide a
  transfer-learning approach. Data augmentation and hyperparameter
  tuning \[cite: 1\] will be investigated to identify possible
  improvements.

------------------------------------------------------------------------

## 3. Dataset Description

- **Dataset:** CIFAR-10 \[cite: 2, 3\]
- **Details:** CIFAR-10 contains 60,000 color images across 10 classes
  (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
  with a resolution of 32 × 32 pixels \[cite: 2, 3\].
  - Training dataset: 50,000 images \[cite: 3\]
  - Testing dataset: 10,000 images \[cite: 3\]

### Data Preprocessing

- Convert images into tensors and normalize them using documented
  channel-wise mean and standard deviation values.
- Split the official training dataset into training and validation
  subsets.
- Keep the official test dataset separate for final evaluation.
- Apply random horizontal flipping and small rotations to training
  images \[cite: 1\].
- Evaluate color jitter as an optional augmentation experiment.
- Resize images and apply the appropriate normalization when using
  pretrained ResNet-18.
- Record random seeds, dataset splits, model settings, and software
  versions for reproducibility.

------------------------------------------------------------------------

## 4. Work-Breakdown Structure (WBS) and Time Estimation

| Task ID | Task Description | Estimated Hours |
|:---|:---|:--:|
| **WBS 1** | Dataset collection and preprocessing, including downloading CIFAR-10, preparing data loaders, and applying augmentation | 8 hrs\[cite: 1\] |
| **WBS 2** | Designing and building the baseline CNN and configuring the ResNet-18 transfer-learning pipeline | 12 hrs\[cite: 1\] |
| **WBS 3** | Training and fine-tuning models, hyperparameter experiments, and performance evaluation | 16 hrs\[cite: 1\] |
| **WBS 4** | Building an interactive application using Streamlit, Gradio, or R Shiny for image classification | 10 hrs\[cite: 1\] |
| **WBS 5** | Writing the final report, documenting methodology, results, plots, and conclusions | 8 hrs\[cite: 1\] |
| **WBS 6** | Preparing presentation slides and visual demonstrations | 6 hrs\[cite: 1\] |
| **Total** | **Estimated Project Effort** | **60 hrs**\[cite: 1\] |

------------------------------------------------------------------------

## 5. Experimental Plan

- Both models will use the same training and validation split and
  evaluation metrics to ensure a fair comparison.
- The validation dataset will be used to select model settings, and the
  test dataset will be used for final evaluation.
- Recorded metrics: Model architecture, preprocessing settings,
  hyperparameter configurations, validation performance, test accuracy,
  macro-precision, macro-recall, macro-F1 score, training time,
  confusion matrices, and loss/accuracy curves.

------------------------------------------------------------------------

## 6. Planned Tools and Technologies

- **Programming Language / Environment:** Python or R (using Jupyter
  Notebook or RStudio)
- **Deep-Learning Framework:** PyTorch, TensorFlow, or compatible R
  packages (e.g., torch/keras in R)
- **Dataset:** CIFAR-10 \[cite: 2, 3\]
- **Models:** Custom CNN and ResNet-18
- **Application Framework:** Streamlit, Gradio, or R Shiny
- **Version Control:** Git and GitHub \[cite: 1\]

------------------------------------------------------------------------

## 7. Scientific References

1.  He, K., Zhang, X., Ren, S., & Sun, J. (2016). *Deep Residual
    Learning for Image Recognition*. CVPR, pp. 770–778\[cite: 1\].
    <https://doi.org/10.1109/CVPR.2016.90>
2.  Krizhevsky, A., Sutskever, I., & Hinton, G. E. (2012). *ImageNet
    Classification with Deep Convolutional Neural Networks*. NeurIPS,
    25\[cite: 1\].
3.  Krizhevsky, A. (2009). *Learning Multiple Layers of Features from
    Tiny Images*. Technical Report, University of Toronto.
