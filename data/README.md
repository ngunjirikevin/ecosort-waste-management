# Dataset Documentation

This directory contains the supporting datasets used in the EcoSort Waste Management Assistant

## 1. Waste Descriptions

**File:** `waste_descriptions.csv`

Contains textual descriptions of waste materials and their corresponding categories

**Purpose:**
- Explore waste descriptions
- Develop a text preprocessing pipeline
- Train and evaluate a waste text classification model

## 2. Waste Policy Documents

**File:** `waste_policy_documents.json`

Contains waste management policy and guideline documents

**Purpose:**
- Prepare policy documents for retrieval
- Generate text chunks and semantic embeddings
- Retrieve relevant information for the RAG component
- Generate contextual recycling and disposal instructions

## 3. RealWaste Image Dataset

**Directory:** `RealWaste/`

The RealWaste image dataset is used to train and evaluate the image classification model

Due to its size, the image dataset is excluded from this GitHub repository

To reproduce the image classification experiments:

1. Obtain the RealWaste dataset from its original distribution source
2. Extract the dataset into this directory
3. Arrange the image folders so that the structure is:

```text
data/
└── RealWaste/
    ├── Cardboard/
    ├── Food Organics/
    ├── Glass/
    ├── Metal/
    ├── Miscellaneous Trash/
    ├── Paper/
    ├── Plastic/
    ├── Textile Trash/
    └── Vegetation/
```

The notebook expects the image dataset at `data/RealWaste/`

## Note

- Large image files are excluded using `.gitignore`