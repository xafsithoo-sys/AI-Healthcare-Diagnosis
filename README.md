# 🧠 Mastering the AI Toolkit – Group Project  
### *AI Applications in Healthcare and Beyond*  

This repository showcases the collaborative efforts of four members exploring how different **AI tools and frameworks** can be applied to solve real-world problems — from **healthcare prediction** to **sentiment analysis** and **ethical AI design**.  

---

## 👥 Team Members and Roles  

| Member | Role | Focus Area | Tools / Frameworks |
|:--------|:------|:------------|:-------------------|
| **Member 1 – Hafsa Hajir** | Data Scientist | Predicting diabetes risk using classical ML | Python, Scikit-learn, Pandas, Matplotlib |
| **Member 2 –brian mwaghogho** | TensorFlow Specialist** | Deep Learning Engineer | Building and training deep neural networks for healthcare prediction | Python, TensorFlow, Keras |
| **Member 3 – Anyira Rodney** | NLP Specialist | Movie review sentiment analysis | SpaCy, Scikit-learn, Pandas |
| **Member 4 – Optimization & Ethics Lead** | Responsible AI & Optimization | Model fine-tuning, fairness, and ethical AI considerations | Python, Scikit-learn, Fairlearn |

---

## 🎯 Project Overview  

Under the theme **“Mastering the AI Toolkit”**, this project explores multiple branches of Artificial Intelligence by dividing tasks among team members to demonstrate:  

- Data-driven healthcare analytics  
- Deep learning applications  
- NLP-driven sentiment classification  
- Ethical AI practices  

Each part contributes to building a holistic understanding of how AI can improve **decision-making, automation, and social good**.

---

## 🩺 Member 1 – Hafsa Hajir (Data Scientist)

This segment focuses on predicting **diabetes risk** using **Scikit-learn** with structured healthcare data.  

### Key Steps:
- Data preprocessing and cleaning  
- Exploratory Data Analysis (EDA)  
- Training a baseline `RandomForestClassifier`  
- Evaluating accuracy, precision, and recall  
- Visualizing feature importance  

### Insights:
- Glucose and BMI were most influential in predicting diabetes.  
- Achieved ~82% accuracy using classical ML.  
- Established a strong baseline for future deep learning improvements.

---

## 🧬 Member 2 – Brian Mwaghogho-TensorFlow Specialist (Deep Learning Engineer)

Developed a **neural network model** using **TensorFlow and Keras** to enhance predictive accuracy on healthcare data.  

### Key Steps:
- Normalized data using feature scaling  
- Implemented multi-layer perceptron (MLP) architecture  
- Applied dropout regularization to prevent overfitting  
- Evaluated model with cross-validation  

### Insights:
- Achieved improved recall compared to baseline ML.  
- Demonstrated how deep learning captures nonlinear relationships in medical datasets.

---

## 💬 Member 3 – Anyira Rodney (NLP Specialist)

Applied **Natural Language Processing (NLP)** to analyze sentiment in movie reviews.  

### Tools:
- SpaCy for tokenization and linguistic processing  
- Scikit-learn for TF-IDF vectorization and model training  
- Pandas for data manipulation  

### Key Steps:
- Cleaned and preprocessed textual data  
- Converted reviews into numerical features (TF-IDF)  
- Trained logistic regression and SVM models  
- Evaluated accuracy and F1-score  

### Insights:
- Achieved strong sentiment classification accuracy (~85%).  
- Highlighted NLP’s versatility beyond healthcare applications.

---

## ⚖️ Member 4 – Optimization & Ethics Lead  

Focused on ensuring **fair, transparent, and reliable** AI performance across all models.  

### Key Focus:
- Identifying potential bias in healthcare and sentiment datasets  
- Using metrics like fairness, recall, and demographic parity  
- Optimizing hyperparameters for improved model generalization  

### Ethical Considerations:
- AI in healthcare must avoid bias in patient data interpretation.  
- Transparency and explainability are key to responsible AI adoption.  

---

## 🧰 Tools and Technologies  

- **Languages:** Python  
- **Frameworks:** Scikit-learn, TensorFlow, SpaCy, Pandas  
- **Visualization:** Matplotlib, Seaborn  
- **Version Control:** GitHub  

---

## 💡 Key Learnings  

- Collaboration across AI subfields improves understanding and innovation.  
- Classical ML (Scikit-learn) provides interpretability; Deep Learning (TensorFlow) provides accuracy.  
- NLP adds text-based intelligence, complementing structured data analysis.  
- Ethical AI ensures fairness, trust, and social responsibility.

---

## 🧭 Ethical Discussion (Group Reflection)

AI has tremendous potential to transform healthcare and information systems, but it must be used responsibly.  
Our team emphasized:  
- Protecting **data privacy and patient confidentiality**  
- Preventing **algorithmic bias** that could disadvantage specific groups  
- Maintaining **model transparency** for explainable decision-making  

Each member contributed ethically:  
- Hafsa ensured proper handling and preprocessing of sensitive health data.  
- Brian  The Deep Learning member avoided overfitting that might lead to false predictions.  
- Rodney anonymized textual data to prevent personal exposure.  
- The Ethics lead evaluated fairness and guided responsible AI use.  

Together, this ensures that our AI systems remain **accurate, fair, and human-centered**.  

---

## 🤝 Collaborators  

A huge thank you to all team members who contributed to the success of this project:  

- 🧠 **[Hafsa Hajir ](https://github.com/xafsithoo-sys)** – Data Scientist  
- 💬 **[Anyira Rodney ](https://github.com/AnyiraRodney)** – NLP Specialist  
-**[Brian Mwaghogho] (https://github.com/brianmwaghogho)**- ⚙️ **TensorFlow Specialist** – Deep Learning Engineer  
- ⚖️ **Ethics & Optimization Lead** – Responsible AI Engineer  

Special appreciation to our instructor and peers for continuous feedback and support during the *Mastering the AI Toolkit* challenge.

---

## 🚀 How to Run  

```bash
# Clone the repository
git clone https://github.com/xafsithoo-sys/Mastering-AI-Toolkit.git

# Navigate into the folder
cd Mastering-AI-Toolkit

# Install dependencies
pip install -r requirements.txt

# Run notebooks or scripts
python member1_diabetes_prediction.py
python member3_sentiment_analysis.py
