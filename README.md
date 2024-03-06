# Chest-XRay-Disease-Diagnosis
 Diagnosing respiratory and cardiovascular conditions from Chest X-Ray images utilizing Convolutional Neural Networks (CNNs), including AlexNet, ResNet18, and Inceptionv3.

 # Introduction
This project focuses on utilizing deep neural networks for medical image diagnosis, specifically with chest X-ray images. In modern healthcare, medical imaging is crucial for assisting medical professionals in making informed diagnostic decisions. Chest X-rays are commonly used but their interpretation can be challenging and time-consuming, even for expert radiologists. The advent of Artificial Intelligence (AI) has brought about a significant transformation in healthcare, leading to this project's goal of utilizing state-of-the-art AI models to aid in diagnosing respiratory and cardiovascular conditions in patients.

The project's methodology involves training advanced Convolutional Neural Networks (CNNs) - namely AlexNet, ResNet18, and Inceptionv3 - with chest X-ray images. The objective is to evaluate these models based on metrics such as Accuracy, Precision, Recall, and F-Score to identify trends in the data and accurately diagnose abnormalities.

# Datasets
Three datasets were used for the project:
1. Chest X-ray Images dataset with 5,856 images of patients with and without pneumonia.
2. Respiratory Disease Classification dataset with 32,687 images of various respiratory diseases, including COVID-19, Lung-Opacity, Viral Pneumonia, Tuberculosis, and Normal.
3. NIH Chest X-rays dataset with 112,120 images representing 15 different abnormalities such as Atelectasis, Consolidation, Pneumothorax, and more.

# TechStack
1. Python: Python is the primary programming language used for developing the deep learning models, data preprocessing, and general scripting.
2. PyTorch: It was used for implementing the Convolutional Neural Networks (CNNs) such as AlexNet, ResNet18, and Inceptionv3 for image classification tasks.
3. CUDA: It was utilized for GPU-accelerated computing, allowing for faster training of deep learning models on compatible NVIDIA GPUs.
4. CuDNN: It was used in conjunction with CUDA to optimize deep learning computations.
5. Pandas: It was used for handling and preprocessing the datasets, particularly the metadata provided in .csv format.
6. NumPy: It was used for handling numerical operations on arrays, when working with image data.
7. Matplotlib and Seaborn: hey were used to create plots and graphs to visualize the performance metrics of the models.
8. Scikit-learn: It was used for evaluating the performance metrics such as accuracy, precision, recall, and F-score of the models.


# Conclusion
In this study, we conducted an ablation study to investigate the effects of different hyperparameters on the performance of Convolutional Neural Networks (CNNs) trained on Dataset 2 for the diagnosis of respiratory diseases using chest X-ray images. Specifically, we focused on two optimization algorithms: Adam and SGD, with varying learning rates.

Our results reveal interesting insights into the impact of these hyperparameters on the performance metrics of the models. When using the Adam optimizer, we observed the highest accuracy of 85.39% with a learning rate of 0.0001, followed closely by 80.76% accuracy with a learning rate of 0.0005. These results indicate that a moderate learning rate in the range of 0.0001 to 0.0005 is optimal for the Adam optimizer in this context.

On the other hand, the SGD optimizer showed lower overall performance compared to Adam, with a maximum accuracy of 71.12% achieved at a learning rate of 0.00001. Additionally, the precision, recall, and F-score metrics were generally higher for the Adam optimizer across different learning rates, indicating its superiority in this experimental setup.

It is important to note that the choice of optimizer and learning rate can significantly impact the performance of deep learning models, particularly in medical image diagnosis tasks. Our findings suggest that for Dataset 2, the Adam optimizer with a learning rate of 0.0001 yielded the best results, achieving a high accuracy along with balanced precision, recall, and F-score.

Overall, this study contributes to the growing body of research on optimizing hyperparameters for CNNs in medical image diagnosis. The insights gained from this ablation study can guide future researchers and practitioners in selecting appropriate hyperparameters to enhance the performance and accuracy of AI models for respiratory disease diagnosis using chest X-ray images.


