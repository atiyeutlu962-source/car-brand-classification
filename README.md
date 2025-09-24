# Car Brand Classification with CNN & Transfer Learning

## Projenin Amacı
Bu proje, farklı otomobil markalarının logolarını içeren görüntüleri derin öğrenme yöntemleri kullanarak sınıflandırmayı amaçlamaktadır. Amaç, görüntü tabanlı marka tanıma modellerinin nasıl geliştirilebileceğini göstermektir.

## Veri Seti
- Kaynak: Kaggle (Car Brand Logos dataset)  
- 8 sınıf: Hyundai, Lexus, Mazda, Mercedes, Opel, Skoda, Toyota, Volkswagen  
- Eğitim seti: ~2013 görüntü  
- Doğrulama seti: 400 görüntü  
- Test seti: 400 görüntü  

## Yöntemler
- **Veri Ön İşleme:** Görseller yeniden boyutlandırıldı, normalize edildi.  
- **Veri Artırma:** Rotation, Flip, Zoom, Color Jitter gibi teknikler uygulandı.  
- **CNN Modeli:** Convolutional katmanlar, pooling, dropout, dense katmanlar ile custom CNN denendi.  
- **Transfer Learning:** MobileNetV2 ve ResNet50 tabanlı modeller ile daha yüksek başarı elde edildi.  
- **Değerlendirme:** Accuracy/Loss grafikleri, Confusion Matrix, Classification Report, Grad-CAM görselleştirmeleri yapıldı.  

## Sonuçlar
- MobileNetV2 tabanlı transfer learning modeli %100 doğrulukla test setini sınıflandırdı.

- Küçük veri seti nedeniyle bu sonuç overfitting göstergesi olabilir.

- Daha büyük ve çeşitlendirilmiş veri setleri ile denenmesi önerilmektedir.

- Ek: EfficientNetB0 ile yapılan denemede test doğruluğu ~%78 seviyesinde gerçekleşti. Bu, modelin aşırı öğrenmeyi azalttığını ve daha genel geçer sonuçlar üretebileceğini göstermektedir.

## Kaggle Notebook
👉 [Notebooku buradan inceleyin](https://www.kaggle.com/code/atiyeutlu/car-brand-classification-f97baf)
