# Text Augmentation using LLMs

### Improving Text Classification by Generating Augmented Text for Under-represented Categories

**Contributors:**  
- **Sid** ([[GitHub](https://github.com/Siddharthj2002)]([[LinkedIn](https://www.linkedin.com/in/siddharthj2002/)]  
- **Sejal Agarwal** ([[GitHub](https://github.com/Sejal135)]([[LinkedIn](https://www.linkedin.com/in/sejal-agarwal/)]  

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Motivation](#motivation)
3. [Dataset](#dataset)
4. [Project Structure](#project-structure)
5. [Usage](#usage)
6. [Collaborators and Version Control](#collaborators-and-version-control)
7. [Results and Evaluation](#results-and-evaluation)
8. [Future Work](#future-work)
9. [References](#references)

---

## Project Overview
This project aims to improve the performance of text classification models by generating augmented text using Large Language Models (LLMs) for under-represented categories. The dataset used is the **AG News dataset**, where we artificially create an imbalance and use LLMs like GPT-4 and BERT to generate additional samples for the minority classes.

---

## Motivation
Many real-world datasets are imbalanced, leading to poor model performance on under-represented classes. In this project, we explore how text augmentation using LLMs can enhance classification performance by generating synthetic text for minority classes. The focus is on improving recall and precision for these classes using various augmentation techniques.

---

## Dataset
We use the [AG News Dataset](https://huggingface.co/datasets/fancyzhx/ag_news) from Hugging Face. It contains 120,000 training samples and 7,600 test samples across four categories:
- **World** 
- **Sports**
- **Business**
- **Science/Technology**

We manually reduce the **Science/Technology** and **Business** categories to create an imbalanced dataset.

---

## Project Structure

The main components of this project are as follows:

```bash
├── data/                   # Folder for raw and processed datasets
├── notebooks/              # Google Colab notebooks
├── models/                 # Trained models
├── src/                    # Python scripts for data processing and model training
├── results/                # Output results (metrics, graphs, etc.)
├── README.md               # Project overview (this file)
└── requirements.txt        # Required Python packages
```

- **notebooks/**: Contains the main Python notebooks for data exploration, augmentation, and model training.
- **src/**: Contains Python scripts for preprocessing, augmentation, and model evaluation.

---

## Usage

### Clone the Repository
To clone and run this project locally:

```bash
git clone https://github.com/your-repo/text-augmentation-using-llms.git
cd text-augmentation-using-llms
```

### Install Dependencies
Install the required Python libraries from `requirements.txt`:

```bash
pip install -r requirements.txt
```

### Run the Notebooks
You can run the Colab notebooks for data augmentation, model training, and evaluation. Make sure you have the correct access to the datasets.

---

## Collaborators and Version Control

### Version Control using GitHub
We are using **GitHub** for version control. Each collaborator works on their own branch and submits pull requests for code review before merging into the main branch.
  
### Collaboration using Google Colab
Both Sid and Sejal are collaborating using **Google Colab** for code development. Colab notebooks are linked to the shared GitHub repository for version control.

- Data is stored in a **Google Drive** shared folder.
- Changes are committed to the repository directly from Colab using **GitHub integration**.

---

## Results and Evaluation

The evaluation focuses on the following metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix**
- **Class-wise Precision and Recall (focus on under-represented classes)**

Visualizations include:
- Precision-Recall curves
- ROC curves
- Confusion matrices

We compare the model performance with and without text augmentation for minority classes.

---

## Future Work
In the future, we aim to:
1. Explore more advanced augmentation techniques.
2. Experiment with other LLMs or pre-trained models.
3. Apply transfer learning to improve the generalization of the models.

---

## References
1. Cegin, J., Simko, J., and Brusilovsky, P. (2024). LLMs vs Established Text Augmentation Techniques for Classification.
2. Dai, H., et al. (2023). AugGPT: Leveraging ChatGPT for Text Data Augmentation.
3. Wei, J., and Zou, K. (2019). EDA: Easy Data Augmentation Techniques for Boosting Performance on Text Classification Tasks.
4. Ubani, S. O., et al. (2023). ZeroShotDataAug: Generating and Augmenting Training Data with ChatGPT.

---

### How to Contribute
If you would like to contribute to this project, feel free to fork the repository and submit a pull request. All contributions are welcome!

---
