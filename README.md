# AYGAZ Global AI Bootcamp Projem

Bu proje, farklı makine öğrenmesi algoritmalarını kullanarak çeşitli veri setleri üzerinde model oluşturma, eğitme ve değerlendirme işlemlerini kapsamaktadır. Proje, eğitim ve test veri setlerini kullanarak doğruluk, F1 skoru, geri çağırma ve kesinlik gibi performans metriklerini hesaplamaktadır.

## İçindekiler
- [Kurulum](#kurulum)
- [Veri Seti](#veri-seti)
- [Modeller](#modeller)
  - [Destek Vektör Makineleri (SVM)](#destek-vektör-makineleri-svm)
  - [LightGBM](#lightgbm)
  - [CNN (Convolutional Neural Network)](#cnn-convolutional-neural-network)
  - [Random Forest](#random-forest)
  - [Decision Tree](#decision-tree)
- [Sonuçlar](#sonuçlar)
- [Katkıda Bulunanlar](#katkıda-bulunanlar)

## Kurulum
Bu projeyi çalıştırmak için aşağıdaki adımları izleyin:

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install -r requirements.txt

2. Proje dosyalarını bilgisayarınıza klonlayın:

cd /path/to/your/directory

git clone https://github.com/myz21/bootcampAI

3.Jupyter Notebook veya herhangi bir Python IDE kullanarak .ipynb uzantılı dosyayı açın ve çalıştırın.

## Veri Seti
Bu projede kullanılan veri setleri:

Fashion MNIST Veri Seti: Moda alanında kullanılan giysi ve aksesuarların sınıflandırılması için kullanılan bir veri setidir. Her biri 28x28 piksel boyutunda 70.000 gri tonlamalı görüntü içerir.
Iris Veri Seti: 3 farklı iris çiçeği türünün özelliklerini içeren bir veri setidir. Her tür için 50 örnek içerir ve toplamda 150 örnekten oluşur.
Veri setleri, sklearn ve keras kütüphaneleri aracılığıyla yüklenmiştir.

## Modeller
### Destek Vektör Makineleri (SVM)
Destek Vektör Makineleri, doğrusal olmayan verileri sınıflandırmak için kullanılan bir algoritmadır. Projemizde, SVM modeli aşağıdaki parametrelerle eğitilmiştir:

Kernel tipi: Linear
Düzenleme parametresi (C): 1.0
### LightGBM
LightGBM, Gradient Boosting algoritmasına dayanan hızlı, dağıtılmış ve yüksek performanslı bir karar ağacı tabanlı öğrenme algoritmasıdır. Fashion MNIST veri seti üzerinde uygulanmıştır. Model eğitimi, veri normalleştirilip düzleştirilerek gerçekleştirilmiştir.

### CNN (Convolutional Neural Network)
Konvolüsyonel Sinir Ağı (CNN), özellikle görüntü tanıma ve sınıflandırma problemlerinde kullanılan derin öğrenme algoritmasıdır. Bu projede, CNN modeli aşağıdaki katmanlardan oluşmaktadır:

Conv2D: 2D evrişim katmanı, görüntülerden özellikler çıkarır.
MaxPooling2D: Özellik haritalarını aşağı örnekler.
Flatten: Çok boyutlu girdileri tek boyutlu vektöre dönüştürür.
Dense: Tam bağlı katman, her nöron tüm girişlerle bağlantılıdır.

### Random Forest
Random Forest, birden çok karar ağacının birleşiminden oluşan bir ansambl öğrenme yöntemidir. Her bir karar ağacı, eğitim verilerinin farklı bir alt kümesi üzerinde eğitilir ve nihai tahmin, tüm ağaçların tahminlerinin ortalaması alınarak elde edilir. Bu yöntem, aşırı uyum (overfitting) riskini azaltır ve genellikle yüksek doğruluk sağlar.

### Decision Tree
Decision Tree, veriyi belirli kurallara göre bölerek sınıflandıran veya regresyon yapan bir makine öğrenmesi algoritmasıdır. Her bir düğüm, veriyi belirli bir özelliğe göre böler ve yaprak düğümler sınıfları veya hedef değerleri temsil eder. Karar ağaçları, verinin yorumlanabilirliğini artırır ancak aşırı uyum riskine sahiptir.

## Sonuçlar
Modelin eğitim ve doğrulama verisi üzerindeki kayıp değerlerinin epoch'lar boyunca azaldığı gözlemlenmiştir. Bu, modelin doğru bir şekilde öğrendiğini göstermektedir. Modelin doğruluk, F1 skoru, geri çağırma ve kesinlik gibi performans metrikleri hesaplanmıştır.

## Katkıda Bulunanlar
Muhammed Yıldız
   
   
