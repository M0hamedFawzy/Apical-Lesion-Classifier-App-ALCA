# Apical Lesion Classifier Application (ALCA)

Ain Shams University  
Faculty of Computer & Information Sciences  
Scientific Computing Department 
###### This repository contains the code for an Apical Lesion Classification app that uses a deep learning model based on DenseNet121 architecture to detect the existence of apical lesions in periapical X-rays. The app includes a Flask server for model inference and a Flutter front-end for user interaction.
## Repository Contents
- `gp_app/`: Contains the Flutter application code.
- `densenet121.ipynb`: Jupyter Notebook for training the DenseNet121 model.
- `server.py`: Flask server script for model inference.

## Features

### Image Manipulation and Annotation
- Includes tools for manipulating and annotating periapical X-ray images.
- Allows users to mark and annotate apical lesions for further analysis.

### Medical Report Management
- Manages medical reports associated with dental x-rays.
- Provides storage and retrieval of reports for multiple patients.

### Accurate and Efficient Apical detection
- Detecting apical lesions in periapical radiographs.
- Utilize deep learning models and Computer Vision techniques.

## Documentation Table of Contents
1. [Introduction](#introduction)
2. [Literature Review](#literature-review)
3. [System Architecture and Methods](#system-architecture-and-methods)
4. [Data Collection](#data-collection)
5. [System Implementation](#system-implementation)
6. [User Manual](#user-manual)
7. [Conclusion and Future Work](#conclusion-and-future-work)


## Introduction

### Problem Definition
Endodontics is a branch of dentistry focused on the pathology of the tooth pulp, which contains sensitive tissue, blood vessels, and nerves. Apical Lesions, also known as apical periodontitis, affect the area surrounding the root apex, causing inflammation. Common types include abscesses, granulomas, and cysts, visible on x-rays as dark shadows.

### Motivation
The project aims to improve diagnostic accuracy and efficiency in dental practices. Traditional methods rely on dental professionals' expertise, which can be subjective and error-prone. By leveraging deep learning, this project aims to develop a consistent, reliable, and faster diagnostic tool for detecting apical lesions.

### Objectives
- Develop a deep learning model for apical lesion detection in radiographic images.
- Integrate the model into a user-friendly application for dental professionals.
- Achieve higher diagnostic accuracy compared to existing methods.

## Literature Review

### Overview
The literature review covers the background of apical lesions, existing diagnostic methods, and recent advancements in deep learning applications in healthcare.

### Related Work
The review compares various approaches and highlights the limitations of current diagnostic methods, emphasizing the need for automated tools.

## System Architecture and Methods

### System Architecture
The system is designed with a three-tier architecture, including data preprocessing, model training, and user interface components.

### Methods and Procedures
A detailed description of the methods used, including data preprocessing techniques, model selection, and training procedures.

## Data Collection

### Dataset Sources
`390 radiographs` were collected from various sources and filtered and labeled with the help of experienced doctors. An additional dataset from the author of "Automatic Classification System for Periapical Lesions in Cone-Beam Computed Tomography" was also used.

### Dataset Description
The final dataset consists of `1390 radiographs` (790 with apical lesions and 600 without).

## System Implementation

### Environment Setup
Details of the software tools and environment setup used for the project.

### Preprocessing
Techniques such as image sharpening, cropping, SMOTE, and CLAHE were applied to enhance the dataset.

### Model Training
Two models, ResNet-50 and DenseNet-121, were trained using ImageNet pre-trained weights. Training achieved an accuracy of 82% on the CBCT dataset and 84% on a combined dataset.

### Evaluation
Using CheXNet pre-trained weights resulted in worse performance compared to ImageNet pre-trained weights.

## User Manual

### Landing Page
Instructions on accessing and navigating the application, including login and sign-up processes.

### Home and Diagnosis Center
Guide to using the home page and diagnosis center for analyzing radiographic images.

### Medical Records
Instructions for managing and accessing patient medical records.

### User Profile
Steps to view and edit user profiles.

## Conclusion and Future Work

### Conclusion
The project demonstrates improved diagnostic accuracy compared to previous works, achieving a highest accuracy of 84%.

### Future Work
Future work includes collecting more balanced data, collaborating with dentists for image annotation, using GANs and Weighted Cross-Entropy Loss to improve performance on imbalanced datasets, and publishing the models and datasets for further research.



This README provides an overview of the Apical Lesion Classifier Application (ALCA) project, summarizing its objectives, methods, and outcomes. For detailed information, please refer to the full documentation.

