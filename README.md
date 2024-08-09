Yapay Sinir Ağları Kullanarak Kemik Erimesi Tanısı

Bu proje, kemik erimesi (osteoporoz) tanısında yapay sinir ağlarının (YSA) etkinliğini değerlendirmeyi amaçlamaktadır. Kemik erimesi, kemik dokusunun yoğunluğunun azalması ve kemik kırılmaları riskinin artmasıyla karakterize edilen bir durumdur. Çalışmada, demografik ve biyolojik özniteliklerin (yaş, cinsiyet, beslenme alışkanlıkları, yaşadığı yer vb.) kemik erimesi tanısındaki rolü anlaşılmaya çalışılmış ve bu tanıda yapay sinir ağlarının kullanılabilirliği araştırılmıştır.


İçindekiler

Giriş

Veri Seti

Veri Görselleştirme

Veri Ön İşleme ve Normalizasyon

Yapay Sinir Ağı Modeli

Veri Seti Bölme

Modelin Oluşturulması

Modelin Eğitilmesi

Sonuçlar

Giriş

Bu projede, kemik erimesi tanısında yapay sinir ağlarının etkinliğini değerlendirmek amaçlanmıştır. Demografik ve biyolojik özniteliklerin kemik erimesi üzerindeki etkileri analiz edilmiş ve bu özniteliklerin bir YSA modeline entegre edilmesiyle tanı doğruluğunun artırılabileceği gösterilmiştir.


Veri Seti

Proje kapsamında kullanılan veri seti, yaş, cinsiyet, kilo, boy, meslek, LDL kolesterol, trigliserit, HDL kolesterol, CRP, WBC, hemoglobin, kreatinin, eğitim durumu, fiziksel aktivite düzeyi, et tüketimi, süt tüketimi, kahve ve alkol tüketimi gibi birçok demografik ve biyolojik özniteliği içermektedir. Hedef değişken ise kemik erimesi durumunu (1 = Kemik erimesi var, 0 = Kemik erimesi yok) ifade etmektedir.

Veri Görselleştirme

Veri setinin yapısını ve özelliklerini daha iyi anlamak amacıyla çeşitli görselleştirme teknikleri kullanılmıştır:

Histogramlar: Özniteliklerin dağılımı analiz edilmiştir.

Kutu Grafikleri: Merkezi eğilimler ve olası aykırı değerler incelenmiştir.

Korelasyon Matrisi: Öznitelikler arasındaki ilişkiler değerlendirilmiştir.

Scatter Plotlar: İki sayısal öznitelik arasındaki ilişkiler görselleştirilmiştir.

Veri Ön İşleme ve Normalizasyon

Veri setindeki öznitelikler, [0, 1] aralığına ölçeklendirilerek min-max normalizasyonu uygulanmıştır. Bu adım, modelin daha hızlı ve istikrarlı bir şekilde eğitilmesine yardımcı olmuştur.

Yapay Sinir Ağı Modeli

Veri Seti Bölme

Veri seti, %70 eğitim ve %30 test olarak ikiye ayrılmıştır. Bu sayede, modelin eğitimi ve test performansı ayrı ayrı değerlendirilmiştir.

Modelin Oluşturulması

Yapay sinir ağı modeli, giriş katmanı, üç gizli katman (15, 20, 15 nöron) ve çıkış katmanı (1 nöron) ile oluşturulmuştur. Levenberg-Marquardt geri yayılım algoritması (trainlm) kullanılarak model eğitilmiştir.

Modelin Eğitilmesi

Model, eğitim verileri üzerinde eğitilmiş ve test verileri üzerinde doğrulanmıştır. Eğitim işlemi sırasında MSE değeri düşük tutulmuş ve modelin doğruluk oranı optimize edilmiştir.

Sonuçlar

Yapay sinir ağı modeli, kemik erimesi tanısında yüksek bir doğruluk oranı elde etmiştir. Elde edilen bulgular, yapay sinir ağlarının klinik uygulamalarda potansiyel bir araç olarak kullanılabileceğini göstermektedir.

