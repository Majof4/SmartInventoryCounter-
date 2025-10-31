# SmartInventoryCounter-

Project Name: Cognitive Clock
Maria Jose Viveros Riquelme
**Tier Selection**
Tier 2 – Image Classification (Medical AI)
This project fits Tier 2 because it applies image classification using CNNs to a real-world healthcare challenge. It uses medical-related data (Clock Drawing Test images) and interprets cognitive patterns that require human-level analysis, making it more complex than basic image labeling tasks.
**Problem Statement**
Early cognitive impairment is often missed because clinicians must manually score the Clock Drawing Test (CDT), a process that is time-consuming and subjective. Many healthcare providers skip it due to limited consultation time, causing delays in early detection of dementia or other cognitive disorders.
**Solution Overview**
The proposed system, Cognitive Clock, uses a Convolutional Neural Network (CNN) to automatically analyze hand-drawn clock images and predict the level of cognitive impairment. By automating CDT scoring, the system provides fast, objective, and consistent evaluations, enabling earlier diagnosis and broader access to cognitive screening tools.
**Technical Approach**
Technique: Image Classification using Convolutional Neural Networks (CNNs)
Model: ResNet-50 or custom CNN architecture
Framework: PyTorch or TensorFlow
Pipeline: Data collection → preprocessing → model training → evaluation → deployment
Justification: CNNs effectively detect spatial and geometric features in human-drawn images, such as number placement and hand alignment, making them ideal for identifying subtle signs of cognitive decline.
**Dataset Plan**
Source: NHATS (National Health and Aging Trends Study) – a U.S. national longitudinal study on aging that includes Clock Drawing Test (CDT) images and corresponding clinical evaluations.
Size: Approximately 500–1,000 labeled images.
Labels: Normal, Mild Impairment, Severe Impairment (based on clinical scoring).
Link (if public): https://nhats.org
Preparation: Resize (224×224), normalize pixel values, and apply augmentation (rotation, brightness, contrast) to improve model robustness.
**Metrics**
Metric Type	Example	Target	Justification
Primary	Model Accuracy	≥ 90 %	Ensures reliable classification for clinical use.
Secondary	Inference Time	< 1 s per image	Enables real-time screening in clinics.
Additional	Precision / Recall	≥ 85 %	Balances false positives and negatives.
Explainability	Grad-CAM Agreement	≥ 80 % clinician alignment	Builds trust and interpretability.
**Week-by-Week Plan**
Week	Task	Milestone
10	Dataset selection, environment setup	Dataset ready
11	Train baseline CNN	Model working
12	Improve with augmentation and tuning	Accuracy ≥ 90 %
13	Build prototype (upload → predict)	Demo ready
14	Documentation and AI log	Completed
15	Presentation and final submission	Final project
Resources Needed
Compute: Google Colab (GPU runtime)
Frameworks: PyTorch, TensorFlow
Dataset Hosting: Roboflow or Kaggle for preprocessing and version control
APIs: Optional deployment via Flask or Streamlit web interface
Cost: $0 (free cloud and open-source tools)
Risks & Mitigation
Risk	Probability	Mitigation
Low accuracy	Medium	Apply data augmentation, hyperparameter tuning, and cross-validation
Missing or inconsistent data	High	Use Roboflow for dataset cleaning or switch to an alternate public dataset
Overfitting	Medium	Use dropout, regularization, and early stopping
Long training time	Low	Utilize Colab GPU and reduce batch size if needed
Limited dataset size	Medium	Apply transfer learning using ResNet-50 pretrained weights

