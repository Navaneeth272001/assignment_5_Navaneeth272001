# Name: Navaneethakrishnan V
# Roll number: DA24S008
## Assignment 5

# Visualizing Data Veracity Challenges in Multi-Label Classification
### Overview
This repository contains a Jupyter Notebook (code.ipynb) that demonstrates the use of non-linear dimensionality reduction techniques—specifically t-SNE and Isomap—to visualize and interpret the Yeast multi-label dataset.

The analysis highlights the challenges of data veracity in real-world machine learning scenarios, including:
- Noisy or ambiguous labels
- Outliers in feature space
- Overlapping classes that make classification difficult

The notebook is designed to be fully reproducible and self-explanatory, with comments and printed outputs at each step.

### Objectives
- Load and preprocess the Yeast dataset (features and labels).
- Identify and analyze the distribution of multi-label combinations.
- Apply t-SNE and Isomap for dimensionality reduction.
- Visualize the structure of the data and assess potential data veracity challenges.
- Discuss findings on the complexity of the data manifold and its implications for classification difficulty.

- **Repository Structure:**

├── code.ipynb # Main notebook for data loading, processing, and visualization
├── README.md # Documentation (this file)
└── yeast/ # Directory containing dataset files (to be created by user)
├── yeast.arff # Feature and label data file
└── yeast.xml # Label description fil

### Dataset Description
- Name: Yeast Dataset (Multi-Label Classification)
- Source: MULAN Repository
- Input: 103 continuous-valued features representing gene expression levels.
- Output: 14 binary label columns representing functional categories of genes.
- The dataset consists of instances where each gene may belong to one or more functional classes.

| Library                 | Purpose                                            |
| ----------------------- | -------------------------------------------------- |
| `pandas`                | Data manipulation and analysis                     |
| `liac-arff`             | Loading ARFF (Attribute-Relation File Format) data |
| `xml.etree.ElementTree` | Parsing XML metadata for labels                    |
| `scikit-learn`          | Standardization, t-SNE, and Isomap algorithms      |
| `matplotlib`            | Data visualization                                 |
| `seaborn`               | Enhanced visualization aesthetics                  |

### Interpretation Guide
- t-SNE Plot: Emphasizes local clusters; helps detect overlapping or noisy label regions.
- Isomap Plot: Highlights the global structure; curvature or complex shapes suggest a nonlinear manifold.
- Highly curved or intertwined manifolds indicate greater classification difficulty due to data complexity and label overlap.