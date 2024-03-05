#f03c15 Dibimbing Final Project - Fetal Health Classification

### *Dataset Link : https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification/data*

![image](https://github.com/hanyprayitno/Dibimbing-Final-Project---Fetal-Health-Classification/assets/153416155/02afd540-aa58-4fc7-83bc-ec2bd70df089)

## 🔎 **Project Overview** 🔎
Final Project ini bertujuan untuk **menganalisis data dalam upaya memperoleh pemahaman mengenai faktor-faktor yang mempengaruhi kesehatan janin** berdasarkan faktor-faktor yang terdapat pada dataset kita seperti; **Percepatan detak jantung, gerakan janin, kontraksi rahim** dan faktor-faktor lain-nya pada kolom dataset kita.

## **Penjelasan Pada Kolom**
- **Baseline Value**: Ini adalah nilai-nilai dasar atau rata-rata dari parameter yang diukur. Dalam hal ini mengacu pada data seperti tekanan darah atau detak jantung yang normal selama kehamilan.
- **Acceleration**: Ini mengacu pada percepatan detak jantung janin dalam respons terhadap rangsangan.
- **Fetal Movement**: Merupakan ukuran dari gerakan janin selama periode waktu tertentu.
- **Uterine Contractions**: Ini mengacu pada kontraksi rahim selama kehamilan.
- **Light Decelerations**, **Severe Decelerations**, **Prolonged Decelerations**: Semua ini mengacu pada perubahan dalam detak jantung janin yang menunjukkan berbagai tingkat keparahan.
- **Abnormal Short Term Variability dan Mean Value Short Term Variability**: Variabilitas ini mengacu pada variasi dalam detak jantung janin yang diukur dalam periode waktu yang singkat.
- **Percentage of Time with Abnormal Long Term Variability dan Mean Value of Long Term Variability**: Ini adalah ukuran variabilitas detak jantung janin dalam jangka waktu yang lebih panjang.
- **Histogram Width, Min, Max, Number of Peaks, Number of Zeroes, Mode, Mean, Median, Variance, Tendency**: Semua ini adalah statistik yang terkait dengan distribusi detak jantung janin.
- **Fetal Health**: Ini mengacu pada penilaian umum tentang kesehatan janin, yang dapat mencakup berbagai faktor.

> Dalam konteks pemantauan kehamilan, data seperti ini digunakan oleh profesional medis untuk memahami kesehatan dan perkembangan janin serta memantau respons terhadap perawatan atau intervensi medis yang mungkin diperlukan.
> Semua data pada kolom bersifat numerik.

## 📒 **Libraries** 📒
```python
import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
import seaborn as sns
from sklearn import preprocessing
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, classification_report, roc_auc_score, confusion_matrix
from sklearn.model_selection import train_test_split, cross_val_score, GridSearchCV, ShuffleSplit
from sklearn.neighbors import KNeighborsClassifier
from sklearn.svm import SVC
from sklearn.feature_selection import SelectKBest
from sklearn.feature_selection import f_classif
from sklearn.model_selection import learning_curve
from sklearn.model_selection import train_test_split
from sklearn.linear_model import Ridge
from sklearn.linear_model import Lasso
```

## 📈 **Learning Curve Overview** 📈
- **KNN**
![image](https://github.com/hanyprayitno/Dibimbing-Final-Project---Fetal-Health-Classification/assets/153416155/4ffbb8b2-8bbc-46cd-a1c0-d7665e672c0f)
- **Random Forest Classifier**
![image](https://github.com/hanyprayitno/Dibimbing-Final-Project---Fetal-Health-Classification/assets/153416155/2d0804df-d6c8-42a1-82c3-5d48e92b88f4)
- **Support Vector Machine**
![image](https://github.com/hanyprayitno/Dibimbing-Final-Project---Fetal-Health-Classification/assets/153416155/5dd5fd5c-effd-4290-b959-73c0953551e5)
