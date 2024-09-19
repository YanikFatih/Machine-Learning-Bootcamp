
# Machine Learning Project: Online Payment Fraud Detection
Bu proje, online olarak yapılan parasal işlemlerde meydana gelen dolandırıcılık vakalarını analiz etmek için bir veriseti kullanmaktadır. Gözetimli ve Gözetimsiz şekilde iki farklı makine öğrenmesi modeli kullanılmıştır. 
# Veri Seti
 https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset

Veri setinin içerdiği verilerde bulunan özellikler şu şekilde:
* step: 1 işlemin 1 saate eşit olduğu bir zaman birimini temsil eder
* type: çevrimiçi işlem türü
* amount: işlem tutarı
* nameOrig: işlemi başlatan müşteri
* oldbalanceOrg: işlemden önceki bakiye
* newbalanceOrig: işlemden sonraki bakiye
* nameDest: işlemin alıcısı
* oldbalanceDest: alıcının işlemden önceki ilk bakiyesi
* newbalanceDest: alıcının işlemden sonraki yeni bakiyesi
* isFraud: dolandırıcılık işlemi

Kullanılan veri seti 6.362.620 satır içermektedir. Projede veri setinin yalnızca ilk 300.000 satırı kullanılmıştır.

# Değerlendirme
Gözetimli öğrenme için **k-En Yakın Komşu (k-Nearest Neighbors - KNN) Sınıflandırıcısı** kullanılmıştır. Oluşturulan modeller ½91.94 (test size 0.3 ve n = 3) ve (test size 0.3 ve n = 7) %92.64 oranında başarım göstermiştir.

Gözetimsiz öğrenme tarafında ise **k-Ortalama (k-Means) Kümeleme** algoritması kullanılmıştır. Aynı zamanda boyut azaltma işlemi de uygulanarak PCA (Principal Component Analysis) ile daha verimli sonuçlar elde edilmesi sağlanmış ve sonuçlar grafik olarak görselleştirilmiştir.

# Kaggle Notebook
https://www.kaggle.com/code/fatihyank/ml-project-online-payment-fraud-detection


