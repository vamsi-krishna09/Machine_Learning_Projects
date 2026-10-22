# Machine_Learning_Projects

# Data Analytics & Machine Learning Projects

This repository has three projects I built with Python in Google Colab: two machine learning projects and one data analysis project from a hackathon. Each project has its own folder with the notebook inside.

---

## 1. Credit Card Default Prediction

**What is the problem?**
Banks lend money through credit cards, and some customers fail to pay back. This is called a "default". If a bank can predict which customers are likely to default, it can reduce its losses. This project builds a model that predicts whether a customer will default, using their past data.

**What data did I use?**
A dataset of about 30,000 credit card customers. The dataset is fetched from ucirepo of id=350

**What did I do?**
1. **Cleaned the data:** handled missing values and outliers, converted categories into numbers (encoding), and scaled the values so models could use them properly.
2. **Trained three models:** Logistic Regression, Random Forest and XGBoost, and compared how well each one predicted defaults.
3. **Tuned the best settings:** used GridSearchCV to test different model settings automatically and pick the best combination.
4. **Judged the models** with accuracy of 0.79, recall of 0.86 for 0 and 0.47 for 1.

**Result**
After tuning, recall improved from 0.58 to 0.63. Recall matters here because it measures how many of the customers who really defaulted the model managed to catch. Missing a defaulter costs a bank more than wrongly flagging a good customer. Random forest performs well than xgboost but tuned xgboost outperforms Random forest

**Tools:** Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib

---

## 2. Plant Disease Detection using a CNN

**What is the problem?**
Plant diseases reduce crop yield, and spotting them early usually needs an expert. This project teaches a computer to look at a photo of a plant leaf and decide whether the plant is healthy or diseased.

**What data did I use?**
A real-world plant image dataset from GitHub https://github.com/pratikkayal/PlantDoc-Dataset.git . Real-world photos are harder than clean lab images because of different lighting, backgrounds and angles.

**What did I do?**
1. **Cleaned and prepared the images** so they could be fed into a neural network.
2. **Used a CNN (Convolutional Neural Network),** which is a type of model built to understand images.
3. **Used transfer learning with a pretrained ResNet model.** ResNet has already learned to recognize general shapes and patterns from millions of images, so I adapted it to plant diseases instead of training from scratch.

**Result**
The model reached an overall F1 score of 0.5526 and accuracy of 0.58, which is better than the results the dataset providers got from their own earlier training which was an accuracy of 31%

**Tools:** Python, PyTorch, ResNet, Pandas, NumPy

---

## 3. Gradient Learning VoltRelay Hackathon (Data Analysis)

**What is the problem?**
In this hackathon, a business was performing poorly and the task was to find out why using the data provided. The goal was not to build a prediction model, but to understand the data and give useful advice.

**What did I do?**
1. **Cleaned and preprocessed** several datasets so they could be combined and analyzed.
2. **Explored the data (EDA)** to find how the business's performance was related to the other information in the data, such as customers, usage, revenue, etc. — add what the datasets covered.
3. **Made charts** with Seaborn to show the patterns clearly.
4. **Gave recommendations** for actions that could improve customer retention (keeping customers) and profits.

**Result**
Network reliability and unit margins cannot be solved by capital expansion; they must be solved by capital efficiency.

True operational turnaround requires shifting capital away from volume (buying more batteries and opening more expensive stations) and toward capability (replacing defective suppliers, retrofitting high-heat cabinets, and enforcing surcharge margin discipline).

*End of Report

**Tools:** Python, Pandas, Seaborn

**Certificate:(https://github.com/vamsi-krishna09/Machine_Learning_Projects/blob/main/Certificate/Data-Analytics-Hackathon-GRD-2026-H74AX0YT.pdf)

---

## How to run a notebook
1. Open the notebook in the project folder and click **Open in Colab**, or use the Colab link under the project.
2. Go to **Runtime → Run all**.
3. Install any missing libraries when Colab asks: `pip install xgboost`.

## About me
C.Vamsi Krishna, B.Tech Chemical Engineering, IIT Madras
ch25b028@smail.iitm.ac.in
