# Lung-Disease-Classification-with-EfficientNetB0

Bu proje, EfficientNetB4 mimarisi kullanılarak akciğer görüntülerinin sınıflandırılmasını amaçlamaktadır. Eğitim ve test işlemleri iki ayrı Python dosyasıyla gerçekleştirilmiştir:

- `Train.py`: Verilen eğitim ve test veri kümeleriyle modeli eğitir.
- `Interface.py`: Eğitilen modeli yükler ve görsel bir arayüz ile kullanıcıdan aldığı görüntüyü sınıflandırır.

---

## 🧠 Kullanılan Teknolojiler

- Python 3.x  
- TensorFlow / Keras  
- EfficientNetB4  
- OpenCV  
- Tkinter  
- NumPy  

---

## 🗂️ Dosya Açıklamaları

### `Train.py`
- EfficientNetB4 modelini kullanarak veri kümesi üzerinde eğitim yapar.
- Eğitim sonrası modeli `.h5` formatında kaydeder (`model.h5`).
- Eğitim ve doğrulama başarı/grafikleri çıkarabilir.
- Model metrikleri: Doğruluk, Kayıp, vb.

### `Interface.py`
- `model.h5` dosyasını yükler.
- Kullanıcıdan bir görüntü seçmesini sağlar (Tkinter arayüzü).
- Seçilen görüntüyü işler ve sınıflandırma sonucunu görsel arayüzde gösterir:
  - Görüntü arayüzde ortada gösterilir.
  - Altında sınıf ismi ve tahmin yüzdesi yazılır.

---

## 🖼️ Örnek Arayüz

![Sample UI](#)  
<!-- Ekran görüntüsünü / arayüz resmini buraya ekleyebilirsin. -->

---

## 🚀 Nasıl Çalıştırılır?

### 1. Eğitim Aşaması
```bash
python Train.py
