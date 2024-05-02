# Stuttering Classification and Therapy System

This project presents a machine learning system designed to classify stuttering and non-stuttering speech segments, along with a user-friendly interface for therapy recommendations.

## Project Overview

This system addresses the challenge of automatic stuttering detection and personalized therapy guidance. It comprises the following key components:

Custom Stuttering Dataset: A meticulously curated dataset containing 815 audio samples categorized into four distinct folders representing different stuttering and non-stuttering speech types.

## Data Preprocessing Pipeline:

### Sample Rate Adjustment: 
Audio samples are converted to a uniform sampling rate of 16,000 Hz for model compatibility.


### Feature Extraction: 
An auto feature extractor efficiently extracts relevant features from the audio data to facilitate model training.


### Dataset Splitting: 
The dataset is divided into training (90%) and testing (10%) sets for model training and evaluation.


## Stuttering Classification Model:

### Fine-Tuned DistilHubert: 
Leverages the pre-trained DistilHubert model from Hugging Face as the foundation, fine-tuned for the task of classifying stuttering in speech samples.


### Training and Optimization: 
The model undergoes training for 10 epochs, iteratively adjusting its parameters based on the training data to enhance its classification accuracy.


## Deployment and User Interface:

### Hugging Face Deployment: 
The trained model is deployed on the Hugging Face platform, ensuring accessibility for users worldwide. You can access the deployed model here: [https://huggingface.co/HareemFatima/distilhubert-finetuned-stutterdetection]

### Gradio User Interface: 
A user-friendly Gradio app interface allows users to interact with the system by uploading audio samples for stuttering classification. You can access the interface from here: [https://huggingface.co/spaces/arisha123/HareemFatima-distilhubert-finetuned-stutterdetection]


### Therapy Generation: 
Integrate a Text-to-Speech model "Massively Multilingual Speech" to generate dynamic therapy recommendations tailored to the user's stuttering type .

## Project Dependencies

### DistilHubert Model:
This project leverages the pre-trained DistilHubert model from Hugging Face for its foundation. You can find more information about DistilHubert here: DistilHubert model on Hugging Face:[https://huggingface.co/ntu-spml/distilhubert]

### Massively Multilingual Speech (MMS) Model:
We also leverage this model from Facebook AI to generate dynamic therapy recommendations based on user input. It allows the system to convert tailored therapy text into natural-sounding audio, enhancing the user experience. You can find more information about it here:[https://huggingface.co/facebook/mms-tts-eng]


## License

This project is licensed under the MIT.
