Karar Ağacı ile Araç Değerlendirme Sınıflandırması
Bu projede, UCI Machine Learning Repository'den alınan Car Evaluation Dataset kullanılarak sıfırdan bir karar ağacı sınıflandırma algoritması geliştirildi. Projenin amacı, farklı araç özelliklerine göre araçların kabul edilebilirlik düzeyini (unacceptable, acceptable, good, very good) doğru şekilde tahmin eden bir model oluşturmaktır.

🔍 Proje Özeti
Karar ağacı algoritması kütüphane kullanılmadan (scikit-learn gibi) tamamen NumPy ve Pandas ile sıfırdan yazılmıştır.

Entropi ve bilgi kazancı hesaplamaları elle yapılmış, ağaç yapısı özyineli olarak inşa edilmiştir.

Modelin aşırı öğrenme (overfitting) sorununu önlemek için budama (pruning) tekniği uygulanmıştır.

Modelin doğruluğu test verisiyle ölçülmüş ve yaklaşık %85 başarı elde edilmiştir.

Eğitim derinliği, karar ağacı görselleştirmeleri ve hata analizleri grafiklerle desteklenmiştir.

 Kullanılan Özellikler
Satın alma fiyatı

Bakım maliyeti

Kapı sayısı

Kişi kapasitesi

Bagaj büyüklüğü

Güvenlik seviyesi

💡 Teknik Detaylar
entropy() ve information_gain() gibi temel fonksiyonlar el ile kodlandı.

DecisionTree sınıfı ile eğitim (fit) ve tahmin (predict) süreçleri yürütüldü.

Kenar durumları (boş veri seti, saf düğüm, vb.) için test senaryoları oluşturuldu.

Modelin öğrenme süreci izlenebilir hale getirilerek hangi özelliklerin daha belirleyici olduğu analiz edildi.

📁 Dosya Yapısı
bash
Copy
Edit
decision_tree.py     # Model kodları
README.md            # Proje açıklaması
 Amaç
Karar ağacı algoritmalarının iç yapısını öğrenmek, algoritmanın nasıl çalıştığını adım adım analiz edebilmek ve veri bilimi alanında temel yapı taşlarından birini uygulamalı olarak deneyimlemek.
