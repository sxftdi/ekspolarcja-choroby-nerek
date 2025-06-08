# Predykcja Przewlekłej Choroby Nerek (CKD) na podstawie danych medycznych

Projekt wykonany w ramach przedmiotu **Eksploracja Danych** na Politechnice Lubelskiej.

## 🎯 Cel projektu
Celem projektu było stworzenie modelu klasyfikacyjnego, który potrafi na podstawie danych klinicznych ocenić ryzyko wystąpienia przewlekłej choroby nerek (CKD). Projekt zawiera pełen proces: od przygotowania danych po budowę i ocenę modeli predykcyjnych.

## 🛠️ Zastosowane techniki i narzędzia
- Czyszczenie danych, imputacja braków (`IterativeImputer`, moda)
- Standaryzacja (`StandardScaler`) i kodowanie zmiennych kategorycznych (Binary Mapping)
- Selekcja cech (`RandomForestClassifier`, `SelectFromModel`)
- Budowa modeli: Logistic Regression, Random Forest, SVM, k-NN, XGBoost
- Kalibracja hiperparametrów (`GridSearchCV`)
- Ocena modeli: accuracy, precision, recall, F1-score, AUC
- Wizualizacja: wykresy ROC, Precision-Recall, macierze pomyłek
- Interpretacja ważności cech (`feature_importance_`)

## 📊 Najlepszy model
Najlepsze wyniki uzyskał model **Random Forest**:
- F1-score: **0.98**
- Accuracy: **97%**
- AUC: **1.00**

Model może służyć jako system wspomagania decyzji dla lekarzy przy wczesnej diagnostyce CKD.

## 👩‍💻 Autorzy
- Diana Kalyniak  
- Zuzanna Winiarska

## 📁 Zawartość repozytorium
- `ckd_prediction_project.ipynb` – główny notebook z kodem i opisem
- `README.md` – opis projektu

## 📌 Dane źródłowe
Zbiór danych: [Chronic Kidney Disease Dataset – UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/chronic_kidney_disease)

