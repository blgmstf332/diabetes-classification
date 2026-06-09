# Diabetes Prediction — Classifier Karşılaştırması

Bu projede **Diabetes (Pima Indians Diabetes)** veri seti üzerinde hastanın diyabet olup olmadığını tahmin etmek için çeşitli sınıflandırma algoritmaları uygulanmış ve karşılaştırılmıştır.

## Veri Seti

- **Veri seti:** Pima Indians Diabetes Dataset
- **Hedef değişken:** `Outcome` (0 = diyabet değil, 1 = diyabet)
- **Eğitim/Test:** `train_test_split` (test seti: 192 örnek)
- **Ölçekleme:** `StandardScaler` bir `Pipeline` içinde (Logistic Regression, SVC, KNN)

## Denenen Modeller

| Model               | Accuracy |
|---------------------|----------|
| AdaBoost            | 0.76     |
| Logistic Regression | 0.69     |
| SVC                 | 0.70     |
| KNN                 | 0.69     |
| Random Forest       | 0.78     |

## Sonuç

En iyi sonucu **Random Forest** ve **AdaBoost** gibi topluluk (ensemble) yöntemleri vermiştir.
