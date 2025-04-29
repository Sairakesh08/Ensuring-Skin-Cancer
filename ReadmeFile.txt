SkinSure AI – Deep Learning for Early Skin Cancer Detection
Author: Sai Rakesh Komatineni


SkinSure AI is a deep learning-powered diagnostic tool developed as part of a postgraduate dissertation by Sai Rakesh Komatineni. The goal of this project is to aid in the early and accurate detection of skin cancer by applying modern machine learning techniques. The system employs Convolutional Neural Networks (CNNs) and transfer learning strategies to classify dermoscopic skin lesion images into benign or malignant categories. By automating and enhancing the diagnostic workflow, this project demonstrates how AI can provide valuable assistance to dermatologists and medical practitioners.

The project is built using the ISIC 2019 Skin Lesion Dataset, which contains over 25,000 high-resolution annotated images. To improve model performance and address class imbalance issues, three versions of the dataset were prepared:

A binary split dataset distinguishing between benign and malignant images.

A balanced dataset using undersampling, where both classes were made equal in size by reducing the majority class.

A balanced dataset using oversampling, where augmentation techniques were used to synthetically increase the minority class.

Multiple models were developed and evaluated across these datasets, including:

A custom-built CNN model

ResNet50 (frozen and fine-tuned)

EfficientNetB0 (fine-tuned)

The CNN model trained on the oversampled dataset yielded the best results, achieving:

Accuracy: 79.63%

ROC-AUC Score: 0.8862

These metrics reflect strong performance in distinguishing between cancerous and non-cancerous lesions. Other evaluation methods such as precision, recall, F1-score, and confusion matrices were also used to analyze and interpret model behavior comprehensively.

The project is implemented in Python, using TensorFlow, Keras, OpenCV, and Matplotlib, with experimentation done on Google Colab. It also includes preprocessing techniques such as image resizing, normalization, and hair removal, as well as visual explanations of model predictions using Grad-CAM.

In the final deployment phase, a user-facing prediction script was built that allows the upload of a dermoscopic image, returning both the predicted label and a Grad-CAM heatmap highlighting critical image regions used by the model.

SkinSure AI demonstrates the potential of AI-driven solutions in medical imaging and serves as an academic and practical reference for researchers and developers exploring AI in dermatology.