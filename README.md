# Predictive Analytics of Diabetes
Building machine learning models for predictive analytics.

![Image](https://julianhealthcare.com/wp-content/uploads/2019/07/Diabetes.jpg)

## 🏷️Metodologi 

The project management methodology used in this project is CRISP-DM. This methodology is one of several methodologies that are often used in the industrial world. Apart from CRISP-DM, there are several project management methodologies, namely Ad Hoc, Waterfall, Agile Scrum & Kanban. 

CRISP-DM (Cross Industry Standard Process for Data Mining) is an approach that describes a standard process for data mining, data science, and machine learning projects. In this methodology, work on a project begins with the business understanding stage so that it can help ensure the project is carried out in accordance with business needs. Another advantage of this methodology is that the work process is iterative, so the work process can be adjusted to the experimental needs of the data science project. This is different from the waterfall methodology which only goes in one direction. 

![CRISP-DM](https://dicoding-web-img.sgp1.cdn.digitaloceanspaces.com/original/academy/dos:418b0f7f4b2dc3d25a68e4f10cca803820230908164632.jpeg)

## 🧭 Project Domain
Domain yang akan dibahas pada project machine learning (*predictive analytics*) ini adalah di bidang **Kesehatan**.

### Latar Belakang
Lifestyle and socio-economic changes due to urbanization and modernization, especially in large cities in Indonesia, have become the main factors causing the increase in the prevalence of degenerative diseases. Several types of degenerative diseases include Diabetes Mellitus (DM), coronary heart disease, hypertension, hyperlipidemia, and others.

Diabetes Mellitus is a common disease in Indonesia. According to the International Diabetes Federation (IDF), Indonesia is ranked 7th out of 10 countries with the highest number of Diabetes Mellitus patients. In 2020, the number of Diabetes Mellitus patients in Indonesia reached 6.2 percent or the equivalent of 10.8 million people and is expected to continue to increase every year.

Even though Diabetes Mellitus can be prevented, 80% of cases still occur due to unhealthy lifestyles. For teenagers, preventive steps can be taken by avoiding behavior that increases the risk of Diabetes Mellitus, because habits from an early age can affect health in old age. Irregular eating patterns and consumption of fast food that is high in fat and low in fiber, vitamins, and minerals can increase the risk of Diabetes Mellitus in the future. Therefore, prevention needs to be done so as not to suffer from DM and to continue living healthily in old age.

Several factors have been shown to be associated with the risk of developing Diabetes Mellitus. First, age is a risk factor that cannot be changed. As a person ages, the risk of developing diabetes also tends to increase. Second, high blood sugar levels during fasting can be an early indication of the risk of diabetes. This can happen because the body may have started to have problems using insulin effectively. Apart from that, there are other factors that need to be considered. By paying attention to these factors, we can better understand our risk of developing diabetes and take steps to prevent it, such as maintaining a healthy diet and exercising regularly.

The application of predictive analytics in predicting Diabetes Mellitus is important because it can help identify individuals who are at high risk of developing this disease. By analyzing various known risk factors, such as age, blood sugar, and various other factors, predictive analytics can provide valuable information for diabetes prevention efforts.

Daftar referensi : 
1. [Hubungan Antara Kepatuhan Minum Obat Pasien Diabetes Mellitus dan Support yang Diberikan Keluarga](https://jurnal.stikessalsabila.ac.id/index.php/jikd/article/view/79/72)
2. [Diabetes melitus](https://juke.kedokteran.unila.ac.id/index.php/juke/article/download/396/397)


## Business Understanding 

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
Dataset yang digunakan pada project machine learning ini adalah [Diabetes dataset]() yang bersumber dari Kaggle. Dataset tersebut berformat csv (comma-separated values) dengan ukuran 23.3 kB. The dataset consists of 768 data records with 9 features. 
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
Data preparation adalah proses mempersiapkan data mentah menjadi format yang sesuai untuk analisis atau pemrosesan lebih lanjut. Berikut adalah beberapa teknik atau metode yang digunakan dalam data preparation pada project ini : 

- Gathering Data 
	Gathering data merupakan tahapan awal pada proses data wrangling. Tahapan ini dilakukan dengan mengumpulkan data yang akan digunakan dalam project machine learning. Pada project ini dataset yang digunakan merupakan data eksternal yang bersumber dari [Kaggle](https://www.kaggle.com/) dan bersifat open-source. Data yang telah diperoleh kemudian diakses atau dibaca dengan menggunakan function yang ada di pandas, yaitu dengan function read_csv().
	
- Assesing Data 
	Assesing data merupakan tahapan dalam data wrangling yang bertujuan untuk mengidentifikasi masalah yang terdapat dalam data dan memastikan data yang digunakan berkualitas. Pada tahapan ini dilakukan identifikasi dataset, termasuk mengecek apakah dataset yang digunakan terdapat missing value, duplicated data, invalid data, inconsistent data, Outliers, dan permasalahan lainnya yang dapat menimbulkan bias pengembangan model machine learning.
	
- Cleaning Data 
	Cleaning data merupakan tahapan dalam data wrangling yang dilakukan dengan tujuan untuk memastikan data tidak mempengaruhi hasil dari analisis atau model machine learning yang dibuat kedepannya. Karena data yang kotor akan menimbulkan bias pada hasil analisis atau model yang tidak akurat. Pada project ini tahapan cleaning data dilakukan meliputi pembersihan missing value apabila ada, duplicated data, menangani outliers, mengangani imbalanced data, dan melakukan standardization. 
	- Melihat jumlah baris dan jumlah kolom
	
	- Melihat data format dan type
	
	- Missing data 
	
	- Duplicated data
	
	- Menampilkan ringkasan statistik dari DataFrame
	
	- Outliers 
		Memeriksa apakah ada outliers dengan menggunakan boxplot. 
	
		GAMBAR  
		
		Menangani outliers dengan menggunakan metode IQR (Inter Quartile Range). IQR tells us the variation in the data set.Any value, which is beyond the range of -1.5 x IQR to 1.5 x IQR treated as outliers.
		GAMBAR 
		
		
		GAMBAR Sesudah 
	
	- Imbalance data
		Gambar pie 
		Based on the image of comparing the number of people with diabetes and non-diabetes, it can be seen that the number of data for people with diabetes is only 34.9% and non-diabetes is 65.1%. This indicates that the data is not balanced (imbalance data). So it is necessary to handle imbalanced data, because unbalanced data can result in bias in the model and accuracy results can be inaccurate.
		
		There are two methods for dealing with imbalance data, namely oversampling and undersampling, depending on the case and dataset you have.

  

Oversampling: Used when we have a small dataset and want to sample more minority classes. Oversampling with SMOTE can help improve model accuracy because it does not lose data, but it can increase the risk of overfitting if not managed properly.

  

Undersampling: Used when we have a large dataset and want to reduce the number of majority class samples. Undersampling can help reduce training time and improve class balance, but it can reduce useful information if majority class samples are randomly removed.

In this case, we will apply the oversamling method because the dataset used is in the small category, so using this method can make the dataset balanced.

		Pada project ini metode yang digunakan yaitu Oversampling menggunakan SMOTE (Synthetic Minority Over-sampling Technique): SMOTE digunakan untuk membuat sampel sintetis dari kelas minoritas (dalam hal ini, kelas "1" dari kolom 'Outcome') agar jumlahnya seimbang dengan kelas mayoritas. Ini membantu mencegah model machine learning menjadi terlalu condong ke arah kelas mayoritas dan meningkatkan performa model untuk kelas minoritas. 
	
		GAMBAR sesudah 
	- Standardization
	Standardisasi adalah proses mengubah data sehingga memiliki mean (rata-rata) nol dan varians (ragam) satu. Tujuan dari standardisasi adalah untuk membuat distribusi data menjadi lebih terpusat di sekitar nilai nol dengan variabilitas yang seragam, yang dapat membantu algoritma machine learning dalam memahami dan memproses data dengan lebih baik. Pada kasus ini StandardScaler dalam scikit-learn digunakan untuk melakukan standardisasi z-score.


## 🎯 Modeling 
Pada project ini algoritma machine learning yang digunakan yaitu  Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree Classifier, and Random forest classification.

- Logistic Regression adalah model sederhana dan mudah diinterpretasikan yang digunakan untuk memprediksi probabilitas terjadinya suatu peristiwa berdasarkan variabel input. Model ini cocok untuk pemodelan hasil biner dan cepat dalam pelatihan dan penggunaannya untuk dataset besar. Namun, model ini mungkin tidak berperforma baik pada masalah yang kompleks dengan banyak fitur atau interaksi, dan rentan terhadap overfitting.

- K-Nearest Neighbors (KNN) adalah model yang intuitif dimana ia memprediksi hasil dengan membandingkan data baru dengan titik data yang ada dalam dataset, memilih label mayoritas dari k tetangga terdekatnya. Meskipun mudah dipahami dan diimplementasikan, KNN memerlukan memori besar untuk menyimpan semua data dan dapat lambat untuk dataset besar, serta sensitif terhadap pencilan.

- Decision Tree Classifier membagi dataset menjadi subset yang lebih kecil berdasarkan fitur-fitur tertentu, dan membuat keputusan berdasarkan struktur pohon yang terbentuk. Model ini mudah dipahami dan diinterpretasikan, tidak memerlukan normalisasi data, dan dapat menangani data kategorikal dan numerik. Namun, decision tree rentan terhadap overfitting dan tidak stabil, karena perubahan kecil dalam data dapat menghasilkan pohon yang berbeda.

- Random Forest Classification adalah model ensemble yang terdiri dari banyak decision tree yang bekerja bersama untuk meningkatkan kinerja dan akurasi prediksi. Model ini mengurangi overfitting dibandingkan dengan decision tree tunggal dan dapat menangani dataset besar dengan banyak fitur. Namun, Random Forest memerlukan lebih banyak waktu untuk pelatihan karena kompleksitas model, dan kurang dapat diinterpretasikan dibandingkan dengan decision tree tunggal.

## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://syarifulmsth.github.io) [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/syariful-musthofa/) [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)

## Feedback
If you have any feedback, please reach out at syarifulm007@gmail.com
