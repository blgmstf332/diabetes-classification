Diabetes Prediction — Classifier Karşılaştırması
Bu projede Diabetes (Pima Indians Diabetes) veri seti üzerinde hastanın diyabet olup olmadığını tahmin etmek için çeşitli sınıflandırma (classification) algoritmaları uygulanmış ve karşılaştırılmıştır. Çalışmaya AdaBoost ile başlanmış, ardından öğrenilen diğer tüm classifier modelleri de aynı veri seti üzerinde denenerek sonuçlar kıyaslanmıştır.
📊 Veri Seti

Veri seti: Pima Indians Diabetes Dataset
Hedef değişken (target): Outcome (0 = diyabet değil, 1 = diyabet)
Eğitim/Test bölünmesi: train_test_split ile ayrıldı (test seti: 192 örnek)
Ölçekleme: İhtiyaç duyan modeller için StandardScaler bir Pipeline içinde uygulandı (Logistic Regression, SVC, KNN)

🤖 Denenen Modeller
Model                 Accuracy (yaklaşık)
AdaBoost              0.76
Logistic Regression   0.69
SVC                   0.70
KNN                   0.69
Random Forest         0.78

⚠️ Yukarıdaki değerler örnek çalıştırmaya aittir. Notebook'u kendin çalıştırdığında random_state'e bağlı olarak küçük farklılıklar görebilirsin. Kesin değerleri notebook çıktısından güncelleyebilirsin.

Her model için accuracy_score, confusion_matrix ve classification_report (precision / recall / f1-score) hesaplanmıştır.
📈 Sonuç
Bu çalışmada en iyi sonucu Random Forest ve AdaBoost gibi topluluk (ensemble) yöntemleri vermiştir.
Bu da diyabet veri seti gibi yapısal (tabular) verilerde ağaç tabanlı topluluk modellerinin tek başına kullanılan basit modellere göre daha iyi performans gösterebildiğini ortaya koymaktadır.
