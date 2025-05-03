# Deepfake Multimodal Detection System

This repository presents an AI-powered deepfake detection system developed as a multimodal classification pipeline capable of analyzing and validating textual, visual, and video content for authenticity. Built by Team SOD (Straight Outta Data), this project addresses the growing threat of AI-generated misinformation by combining state-of-the-art models across different modalities into a unified, scalable framework.

## Project Highlights
- **Multi-Model Approach:** Incorporates Vision Transformer (ViT) for image classification, a fine-tuned BERT (bert-base-uncased) model for text classification, and a hybrid CNN-LSTM model for video analysis.
- **Data Sources:** Utilizes DeepFakeNews dataset (Zenodo) for images and metadata, and FaceForensics++ for video deepfakes. Data is stored and queried from AWS S3 using Athena and Glue.
- **Data Engineering:** Includes preprocessing pipelines for text, images, and videos. Video preprocessing features face-frame extraction, temporal alignment, and consistent formatting.
- **Evaluation & Metrics:** Achieved high model accuracy across all modalities — including 99% training and 97% test accuracy on the image model and 100% emergency recall on text triage classification.
- **Visualization & Reporting:** Integrated Power BI dashboards and Gradio UI to support explainability, demo interactions, and stakeholder engagement.
- **Cloud-Based Storage & Querying:** Metadata and raw data are maintained in AWS S3, cataloged with AWS Glue Crawlers, and accessed via AWS Athena for high availability and schema detection.

## Tools & Frameworks
- Python, PyTorch, HuggingFace Transformers, OpenCV, AWS (Athena, Glue, S3), Streamlit, Gradio, Power BI
- Model Architectures: ViT, BERT, LSTM, EfficientNet, ResNeXt

## Purpose
This solution offers an extensible foundation for combating disinformation through automated multimodal analysis. It is designed to be used in journalism, social platforms, and content moderation systems to flag and verify fake media content in real-time.

