# Traditional Machine Learning Classification on Balanced Dataset

Bu projede, dengelenmiş bir veri kümesi (`balanced_update_data_dt.csv`) üzerinde çeşitli geleneksel makine öğrenmesi sınıflandırma algoritmaları kullanılarak performans karşılaştırması yapılmıştır.

## Kullanılan Algoritmalar

- Decision Tree (Karar Ağacı)
- Support Vector Machine (SVM)
- Naive Bayes
- Random Forest

## Adımlar

1. **Veri Yükleme ve Hazırlık:**  
   Veri kümesi yüklenmiş, `class` sütunu hedef değişken olarak ayrılmıştır. Eğitim ve test kümeleri %80-%20 oranında bölünmüştür.

2. **Sınıf Dağılımının Görselleştirilmesi:**  
   Sınıf dağılımı çubuk grafikle gösterilerek dengenin sağlandığı doğrulanmıştır.

3. **Korelasyon Isı Haritası:**  
   Hedef değişken ile öznitelikler arasındaki ilişki ısı haritası ile görselleştirilmiştir.

4. **Model Eğitimi ve Değerlendirme:**  
   Her bir model, eğitim verisi ile eğitilip test verisi üzerinde değerlendirilmiştir. Değerlendirme metrikleri:
   - Accuracy (Doğruluk)
   - Precision, Recall, F1-Score
   - Confusion Matrix (Karışıklık Matrisi)

5. **Görselleştirme:**  
   Her model için karışıklık matrisi ayrı ayrı ısı haritası olarak çizdirilmiştir.

## Gereksinimler

```bash
pip install pandas matplotlib seaborn scikit-learn
