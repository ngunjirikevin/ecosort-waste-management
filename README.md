# EcoSort: AI-Powered Waste Management Assistant

## Project Overview

EcoSort is an AI-enabled waste management assistant designed to help users identify waste materials and access relevant recycling and disposal guidance

The project combines **Computer Vision**, **Natural Language Processing (NLP)**, and **Retrieval-Augmented Generation (RAG)** to provide waste identification and policy-informed recommendations

Users can provide an image of a waste item or a text description. The system predicts the waste category and retrieves relevant guidance to help users understand how the material should be handled

## Problem Statement

Improper waste disposal contributes to environmental pollution and reduces opportunities for recycling and material recovery

People may struggle to identify different waste materials and determine the appropriate disposal methods. Existing waste management information can also be difficult to access or understand

EcoSort explores how machine learning and AI can make waste identification and recycling guidance more accessible

## Project Objectives

The project aims to;

1. Develop an image classification model capable of identifying waste materials
2. Build a text classification model that categorizes waste from written descriptions
3. Implement a document retrieval system that finds relevant waste management policies and guidelines
4. Generate contextual recycling and disposal instructions using retrieved documents
5. Integrate the models into a unified waste management assistant

## Core Components

| Component | Purpose | Approach |
|---|---|---|
| Image Classification | Identify waste from uploaded images | CNN with MobileNetV2 transfer learning |
| Text Classification | Categorize waste from written descriptions | TF-IDF and Multinomial Naive Bayes |
| Policy Retrieval | Retrieve relevant waste management information | Sentence Transformers and semantic similarity |
| Instruction Generation | Generate guidance using retrieved policy context | FLAN-T5 and RAG |
| System Integration | Combine the components into one assistant | Python |

## Dataset Overview

The project uses three datasets;

- **RealWaste:** An image dataset containing nine waste categories, used to train and evaluate the image classification model
- **Waste Descriptions:** A collection of textual waste descriptions used to develop the NLP classification model
- **Waste Policy Documents:** Policy and guideline documents used to build the retrieval-augmented generation component

The large RealWaste image dataset is excluded from this GitHub repository because of its size. Instructions for obtaining and arranging the dataset are provided in the `data/README.md` file

## Technologies and Tools

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas and NumPy
- Sentence Transformers
- Hugging Face Transformers
- Matplotlib and Seaborn
- Jupyter Notebook
- Git and GitHub

## Project Workflow

1. Explore and prepare the image, text, and policy datasets
2. Develop and evaluate the image classification model
3. Develop and evaluate the text classification model
4. Implement semantic document retrieval and response generation
5. Integrate the components into the EcoSort assistant
6. Test the integrated system

## Repository Structure

```text
ecosort-waste-management/
│
├── data/
│   ├── README.md
│   ├── waste_descriptions.csv
│   └── waste_policy_documents.json
│
├── waste_management_summative.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

The RealWaste image directory is stored locally and excluded through `.gitignore`


## Future Improvements

Potential improvements include;

- Expanding the waste image dataset
- Improving classification performance across waste categories
- Developing a user-friendly web application
- Exploring deployment and real-world testing
