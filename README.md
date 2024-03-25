# Diabetes Predictive Analytics

Building machine learning models for predictive analytics.

![Image](https://julianhealthcare.com/wp-content/uploads/2019/07/Diabetes.jpg)

## 🏷️ Methodology 

The project management methodology used in this project is CRISP-DM. This methodology is one of several methodologies that are often used in the industrial world. Apart from CRISP-DM, there are several project management methodologies, namely Ad Hoc, Waterfall, Agile Scrum & Kanban. 

CRISP-DM (Cross Industry Standard Process for Data Mining) is an approach that describes a standard process for data mining, data science, and machine learning projects. In this methodology, work on a project begins with the business understanding stage so that it can help ensure the project is carried out in accordance with business needs. Another advantage of this methodology is that the work process is iterative, so the work process can be adjusted to the experimental needs of the data science project. This is different from the waterfall methodology which only goes in one direction. 

![CRISP-DM](https://dicoding-web-img.sgp1.cdn.digitaloceanspaces.com/original/academy/dos:418b0f7f4b2dc3d25a68e4f10cca803820230908164632.jpeg)

## 🧭 Project Domain
Domain yang akan dibahas pada project machine learning (*predictive analytics*) ini adalah di bidang **Kesehatan**.

### Background 
Lifestyle and socio-economic changes due to urbanization and modernization, especially in large cities in Indonesia, have become the main factors causing the increase in the prevalence of degenerative diseases. Several types of degenerative diseases include Diabetes Mellitus (DM), coronary heart disease, hypertension, hyperlipidemia, and others.

Diabetes Mellitus is a common disease in Indonesia. According to the International Diabetes Federation (IDF), Indonesia is ranked 7th out of 10 countries with the highest number of Diabetes Mellitus patients. In 2020, the number of Diabetes Mellitus patients in Indonesia reached 6.2 percent or the equivalent of 10.8 million people and is expected to continue to increase every year.

Even though Diabetes Mellitus can be prevented, 80% of cases still occur due to unhealthy lifestyles. For teenagers, preventive steps can be taken by avoiding behavior that increases the risk of Diabetes Mellitus, because habits from an early age can affect health in old age. Irregular eating patterns and consumption of fast food that is high in fat and low in fiber, vitamins, and minerals can increase the risk of Diabetes Mellitus in the future. Therefore, prevention needs to be done so as not to suffer from DM and to continue living healthily in old age.

Several factors have been shown to be associated with the risk of developing Diabetes Mellitus. First, age is a risk factor that cannot be changed. As a person ages, the risk of developing diabetes also tends to increase. Second, high blood sugar levels during fasting can be an early indication of the risk of diabetes. This can happen because the body may have started to have problems using insulin effectively. Apart from that, there are other factors that need to be considered. By paying attention to these factors, we can better understand our risk of developing diabetes and take steps to prevent it, such as maintaining a healthy diet and exercising regularly.

The application of predictive analytics in predicting Diabetes Mellitus is important because it can help identify individuals who are at high risk of developing this disease. By analyzing various known risk factors, such as age, blood sugar, and various other factors, predictive analytics can provide valuable information for diabetes prevention efforts.

Daftar referensi : 
1. [Hubungan Antara Kepatuhan Minum Obat Pasien Diabetes Mellitus dan Support yang Diberikan Keluarga](https://jurnal.stikessalsabila.ac.id/index.php/jikd/article/view/79/72)
2. [Diabetes melitus](https://juke.kedokteran.unila.ac.id/index.php/juke/article/download/396/397)
3. [Analisis Faktor Resiko Penyebab Terjadinya Diabetes Melitus Tipe 2 Pada Wanita usia Produktif Di Puskesmas Wawonasa](https://ejournal.unsrat.ac.id/index.php/ebiomedik/article/view/4554)


## 📌 Business Understanding 

### Problem Statement 
Diabetes Mellitus is one of the degenerative diseases whose prevalence continues to increase, including in Indonesia. The main problem faced is the difficulty in detecting and preventing diabetes early, which can lead to serious complications if not addressed properly.

### Goals 
1.  Collecting and cleaning diabetes data that includes relevant risk factors.
2.  Identifying the most influential features in predicting Diabetes Mellitus, including conducting statistical analysis and data exploration to understand the relationships between these features.
3.  Building a machine learning model that can predict the likelihood of someone experiencing Diabetes Mellitus based on known risk factors.
4.  Evaluating models to select the best model based on appropriate evaluation metrics, such as accuracy, precision, recall, and F1-score.

### Solution Statements
1.  Analyzing and cleaning available diabetes data for use in model development.
2.  Identifying the most influential features in predicting Diabetes Mellitus.
3.  Building and testing several machine learning models to predict Diabetes Mellitus.
4.  Evaluating models and selecting the best model based on appropriate evaluation metrics.

## 📚 Data Understanding 
Dataset yang digunakan pada project machine learning ini adalah [Diabetes dataset](https://www.kaggle.com/datasets/mathchi/diabetes-data-set) yang bersumber dari Kaggle. Dataset tersebut berformat csv (comma-separated values) dengan ukuran 23.3 kB. The dataset consists of 768 data records with 9 features. 
The following is a table containing details of the Diabetes Dataset dataset:

| Feature | Description |
|------------------------|------------------------------------------------------------------------|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration a 2 hours in an oral glucose tolerance test|
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body mass index (weight in kg/(height in m)^2) |
| DiabetesPedigreeFunction | Diabetes pedigree function |
| Age | Age in years |
| Outcome | Class variable (0 or 1) |

## 📚 Data Preparation 
Data preparation is the process of preparing raw data into a suitable format for further analysis or processing. The following are several techniques or methods used in data preparation on this project:

- Gathering Data 
Gathering data is the initial stage in the data wrangling process. This stage is carried out by collecting data that will be used in the machine learning project. In this project the dataset used is external data sourced from [Kaggle](https://www.kaggle.com/) and is open-source. The data that has been obtained is then accessed or read using the function in Pandas, namely the read_csv() function.
	
- Assesing Data 
Assessing data is a stage in data wrangling which aims to identify problems contained in the data and ensure the quality of the data used. At this stage, dataset identification is carried out, including checking whether the dataset used contains missing values, duplicated data, invalid data, inconsistent data, outliers, and other problems that can cause bias in the development of machine learning models.
	
- Cleaning Data 
Cleaning data is a stage in data wrangling which is carried out with the aim of ensuring that the data does not affect the results of the analysis or machine learning models that are created in the future. Because dirty data will cause bias in analytical results or inaccurate models. In this project, the data cleaning stages include cleaning missing values ​​if any, duplicated data, handling outliers, handling imbalanced data, and carrying out standardization.
	- View the number of rows and number of columns
 	<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/Capture1.PNG?raw=true" alt="Diabetes"  width="300"></p>    
	- View data format and type
	<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/Capture2.PNG?raw=true" width="300"></p>
	- Missing data 
	<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/Capture3.PNG?raw=true " width="300" ></p>
	- Duplicated data
	<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/Capture4.PNG?raw=true"  width="300"></p>
	- Displays summary statistics from a DataFrame
	<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/Capture5.PNG?raw=true"  width="300"></p>
- Outliers <br>
Check if there are outliers by using a boxplot. 
<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/outliersBefore.png?raw=true"></p> Handle outliers using the IQR (Inter Quartile Range) method. IQR tells us the variation in the data set. Any value, which is beyond the range of -1.5 x IQR to 1.5 x IQR is treated as outliers.
![iqr](https://dicoding-web-img.sgp1.digitaloceanspaces.com/original/academy/dos:4943e2b65e16d68cf187164fae50174b20231012141616.png)
Result after handling outliers :
<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/outliersAfter.png?raw=true"  ></p>

- Imbalance data
<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/imbalancedBefore.png?raw=true" ></p> Based on the image of comparing the number of people with diabetes and non-diabetes, it can be seen that the number of data for people with diabetes is only 34.9% and non-diabetes is 65.1%. This indicates that the data is not balanced (imbalance data). So it is necessary to handle imbalanced data, because unbalanced data can result in bias in the model and accuracy results can be inaccurate. There are two methods for dealing with imbalance data, namely oversampling and undersampling, depending on the case and dataset you have.
	- Oversampling: Used when we have a small dataset and want to sample more minority classes. Oversampling with SMOTE can help improve model accuracy because it does not lose data, but it can increase the risk of overfitting if not managed properly.
 	- Undersampling: Used when we have a large dataset and want to reduce the number of majority class samples. Undersampling can help reduce training time and improve class balance, but it can reduce useful information if majority class samples are randomly removed.<br><br>In this case, we will apply the oversamling method because the dataset used is in the small category, so using this method can make the dataset balanced. In this project, the method used is Oversampling using SMOTE (Synthetic Minority Over-sampling Technique): SMOTE is used to create synthetic samples from the minority class (in this case, class "1" from the 'Outcome' column) so that the number is balanced with the majority class. This helps prevent the machine learning model from being too skewed towards the majority class and improves model performance for the minority class.<br><br>
    Result after handling imbalanced datasets
    <br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/imbalancedAfter.png?raw=true"  width="300"></p>	

- Standardization
<br><img src ="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/featureScaling.png?raw=true" ></p>	Standardization is the process of changing data so that it has a mean (average) of zero and a variance (variance) of one. The goal of standardization is to make the data distribution more centered around the zero value with uniform variability, which can help machine learning algorithms understand and process the data better. In this case StandardScaler in scikit-learn is used to standardize z-scores.

- Data Splitting 
Data splitting is the process of dividing a dataset into two or more different parts for use in certain stages of the data analysis process, such as model training, model validation, and model testing. In this project, data splitting uses the Train-test split method. Train-test split is a technique for dividing a dataset into two parts: one for training the model (training set) and the other for testing the model (test set).

## 🎯 Modeling 
In this project the machine learning algorithms used are Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree Classifier, and Random forest classification.

- Logistic Regression is a statistical model that uses the logistic function, or logit function, in mathematics as the equality between x and y. The logit function maps y as a sigmoid function of x. The advantage of this model is that it is easy to understand and implement. Suitable for modeling binary data (two classes).
![image](https://d1.awsstatic.com/sigmoid.bfc853980146c5868a496eafea4fb79907675f44.png)
![image](https://d1.awsstatic.com/S-curve.36de3c694cafe97ef4e391ed26a5cb0b357f6316.png)
The following is the application of the algorithm in this project:
	> LogisticRegression(max_iter=1000)

- K-Nearest Neighbors (KNN) is a relatively simple algorithm compared to other algorithms. The KNN algorithm uses 'feature similarity' to predict the value of each new data. In other words, each new data is assigned a value based on how similar the points are in the training set.
KNN works by comparing the distance of one sample to another training sample by selecting k nearest neighbors (where k is a positive number). Well, that's why this algorithm is called K-nearest neighbors (a number of k nearest neighbors). KNN can be used for classification and regression cases. The advantage of this algorithm is that it is simple and intuitive. Suitable for datasets that are not too large and do not have a complex structure. In this project the parameters used are as follows: 
	> KNeighborsClassifier(n_neighbors=11, p=2, metric='euclidean')

	![image](https://miro.medium.com/v2/resize:fit:640/format:webp/0*2_qzcm2gSe9l67aI.png)

- Decision Tree Classifier is a tree structure consisting of nodes that represent decisions and branches that represent the consequences of those decisions. Each node in the decision tree represents a variable in the dataset that influences the decision and its consequences. The advantage of this algorithm is that it is easy to understand and can handle categorical and numerical data. Allows visual interpretation. In this project the parameters used are as follows:
	> DecisionTreeClassifier(random_state=42)

	![image](https://images.datacamp.com/image/upload/v1677504957/decision_tree_for_heart_attack_prevention_2140bd762d.png)
  
	Decision trees are one of the most popular machine learning models and are most often used in classification and regression problems. Used to divide data into smaller and more homogeneous subsets until a result or decision is obtained.
	
- Random Forest Classification is an ensemble model consisting of many decision trees that work together to improve prediction performance and accuracy. This model reduces overfitting compared to a single decision tree and can handle large datasets with many features. However, Random Forest requires more time to train due to the complexity of the model, and is less interpretable compared to a single decision tree. The advantage of this algorithm is that it can overcome the overfitting problem that commonly occurs in decision trees. Able to handle large datasets with many features. The following are the parameters used in this project : 
	> RandomForestClassifier(n_estimators=100)
	
	![image](https://blog.myskill.id/wp-content/uploads/2023/10/972e598f-8afe-4e6a-91d6-4799fba0a55f_2224x1053.png)

## 📈 Evaluation 
Pada project ini evaluasi model menggunakan Classification Report. The classification report is part of the scikit-learn module in python. It is report containing the key metrics in a classification problem and showing the quality of the predictions.

The classification report visualizer displays the precision, recall, F1, and support scores for the model.
- **Precision —** The percentage of correctly classified results among that class.
- **Recall —** The number of true positive cases found over the total number of positive cases found (true positives + false negatives).
- **F1-score —**  The harmonic mean of precision and recall. The F1-score will always be between 1.00 and 0.00 with 1.00 being the best score.
- **Support —** The number of occurrences of the class in the dataset.

Based on the results of the analysis and development of machine learning models that have been carried out, the machine learning model with the best accuracy and evaluation results is the **Random Forest Classifier** algorithm.
 
<p align="center"><img src="https://github.com/SyarifulMsth/predictive-analytics-of-diabetes/blob/main/image/accuracy.PNG?raw=true" height="200px" style="display:block; margin:auto;"></p>


## Daftar Pustaka


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://syarifulmsth.github.io) [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/syariful-musthofa/) [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)

## Feedback
If you have any feedback, please reach out at syarifulm007@gmail.com
