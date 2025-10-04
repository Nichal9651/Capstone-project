# Capstone-project
Working on "AI-Powered Cancer Diagnosis and Preventive Care Assistant"
with BLIP and pre-trained LLM


##DataSet:https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic

##Code: [[https://colab.research.google.com/drive/199NG6zWJH1D4oxNjidC-nCs5ZOSrizzq?usp=sharing](https://colab.research.google.com/drive/17Ein4H5CtNLCVTsZaRek8LfilWcfwSgr)](https://colab.research.google.com/drive/17Ein4H5CtNLCVTsZaRek8LfilWcfwSgr?usp=sharing)

🩺 Skin Cancer Detection using BLIP + LLM
📌 Overview

This project integrates BLIP (Bootstrapping Language-Image Pretraining) for image captioning with a Large Language Model (LLM) to classify skin cancer images into 9 classes.

BLIP generates a descriptive caption from the skin lesion image.

LLM (Flan-T5) takes the caption and predicts the most likely cancer type with reasoning.

The system demonstrates a vision-language pipeline without fine-tuning, using pretrained models.

🎯 Objectives

Use BLIP to extract visual features as natural language captions.

Classify skin lesions into 9 classes using an LLM.

Evaluate the performance using accuracy, precision, recall, and F1-score.

Provide explainable outputs with reasoning.

🧾 Dataset

Source: Kaggle – Skin cancer ISIC: 9 Classes Dataset

Classes:

Actinic Keratosis

Basal Cell Carcinoma

Dermatofibroma

Melanoma

Nevus

Seborrheic Keratosis

Squamous Cell Carcinoma

Vascular Lesion

Normal

⚙️ Tools & Technologies

Python 3.10+

PyTorch

Hugging Face Transformers

BLIP (Salesforce/blip-image-captioning-base)

FLAN-T5 (google/flan-t5-large)

Pandas, Scikit-learn, Matplotlib

Google Colab / Kaggle Notebooks

🚀 Workflow

Dataset Loading: Load ISIC dataset & prepare image-label mapping.

BLIP Captioning: Generate descriptive captions for images.

Prompt Construction: Create structured prompts with possible cancer labels.

LLM Classification: Use FLAN-T5 to classify captions into cancer types.

Evaluation: Compare predictions with ground truth & compute accuracy.

📊 Results

Captions generated successfully for all images.

LLM provided class predictions with reasoning.

Achieved measurable accuracy (baseline, since no fine-tuning).

Example output:

{
  "caption": "A close-up image of a dark irregular skin lesion.",
  "predicted_label": "melanoma",
  "rationale": "The lesion is irregular and dark, which is characteristic of melanoma."
}

🔮 Future Enhancements

Fine-tune BLIP and LLM models for domain-specific accuracy.

Use premium GPU (Colab Pro / A100) for faster training.

Try advanced LLMs like Grok AI or GPT-4 for better reasoning.

Deploy as a web application for doctors/researchers.

📚 References

Salesforce BLIP

Google FLAN-T5

Kaggle ISIC Dataset

Hugging Face Transformers

PyTorch
