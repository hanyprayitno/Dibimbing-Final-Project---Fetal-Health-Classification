# 🚑 Dibimbing Final Project - Fetal Health Classification 🚑

## *Dataset Link : https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification/data*

![alt text](https://freepngimg.com/download/python_logo/5-2-python-logo-png-image.png) ![alt text](data:image/png;base64,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)

## Project Overview
Final Project ini bertujuan untuk **menganalisis data dalam upaya memperoleh pemahaman mengenai faktor-faktor yang mempengaruhi kesehatan janin** berdasarkan faktor-faktor yang terdapat pada dataset kita seperti; **Percepatan detak jantung, gerakan janin, kontraksi rahim** dan faktor-faktor lain-nya pada kolom dataset kita.
