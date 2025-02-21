
# **Phishing Website Detection Using Machine Learning**  

## **Objective**  
Phishing websites are a common cybersecurity threat, designed to mimic legitimate sites and steal sensitive user information. This project aims to develop machine learning models to predict phishing websites based on extracted URL and webpage content features. The dataset consists of both phishing and benign URLs, and multiple machine-learning models are trained and evaluated for performance.  
<img width="1344" alt="image" src="https://github.com/user-attachments/assets/4339650d-f2fe-4806-a3fd-3173f65db683" />

<img width="1344" alt="image" src="https://github.com/user-attachments/assets/a7a3d455-e434-4fa2-a662-86995772e5ed" />


## INTERNAL

<img width="1344" alt="Screenshot 2025-02-21 at 4 39 31 PM" src="https://github.com/user-attachments/assets/c530adc7-18ab-4f16-b9ac-696efc76708b" />
<img width="1344" alt="image" src="https://github.com/user-attachments/assets/e0527b88-525e-4c5a-be8e-08394d68f562" />

## **Data Collection**  
The dataset for this project is compiled from two primary sources:  

- **Phishing URLs** were collected from an open-source phishing database, which is updated regularly to provide the latest phishing websites. A random selection of 5,000 phishing URLs was used for training.  
- **Legitimate URLs** were sourced from a publicly available dataset that contains various types of URLs, including benign, spam, phishing, malware, and defacement. For this project, 5,000 legitimate URLs were selected.  

## **Feature Extraction**  
Features were extracted from URLs and webpage content to enhance model accuracy. The extracted features fall into three categories:  

1. **Address Bar-Based Features** – Includes 9 features related to the structure of the URL, such as the presence of special characters, domain age, and HTTPS usage.  
2. **Domain-Based Features** – 4 features derived from domain-related attributes, such as WHOIS information and IP-based detection.  
3. **HTML & JavaScript-Based Features** – 4 features extracted from webpage content, including embedded scripts, iframe usage, and suspicious JavaScript functions.  

A total of 17 features were extracted and stored for model training.  

## **Model Training & Evaluation**  
The dataset was split into an **80-20** ratio, with 8,000 samples used for training and 2,000 for testing. Since this is a **supervised classification problem**, multiple machine learning models were implemented to classify URLs as phishing (1) or legitimate (0).  

The following models were trained and evaluated:  

- **Decision Tree**  
- **Random Forest**  
- **Multilayer Perceptrons (MLP)**  
- **XGBoost**  
- **Autoencoder Neural Network**  
- **Support Vector Machines (SVM)**  

Each model's performance was assessed, and results were compared to determine the most effective approach.  

## **Results & Best Performing Model**  
After evaluating all models, the **XGBoost Classifier** demonstrated the highest accuracy of **86.4%**, making it the best-performing model for phishing website detection.  

## **Next Steps & Future Work**  
This project can be extended further with practical implementations, such as:  

- Developing a **browser extension** that integrates the trained model to detect phishing websites in real-time.  
- Creating a **GUI-based tool** where users can input a URL and receive an instant classification (legitimate or phishing).  

Currently, efforts are underway to develop the browser extension, and updates will be provided as the project progresses.  

## **Conclusion**  
This project successfully demonstrates how machine learning techniques can be leveraged to detect phishing websites with high accuracy. By integrating advanced classification models and feature extraction techniques, this approach can enhance online security and help protect users from cyber threats.  

---
