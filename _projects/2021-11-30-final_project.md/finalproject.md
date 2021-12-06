---
layout: post
title: Final Projesi
subtitle: 
categories: final_projesi
authors: [Cemal Efe Gayir, Rutkay Var]
tags: [final_projesi]
slug: final_projesi
---

CS 101 Bahar 2021'in 6 haftasını geride bıraktık! Şimdiye kadar inanılmaz bir gelişme gösterdiğiniz ve 
programı takip ettiğiniz için hepinizi tebrik ederiz. Programın son 2 haftasında Final Projesi yaparak 
öğrendiklerinizi bir oyunla ölümsüzleştireceksiniz. 

Aşağıda Final Projesi ile ilgili verilen uzuun açıklamayı dikkatlice okuyun, başarılar.

## Başlangıç Kodları
Final Projesine ait başlangıç kodlarına [buradan](https://drive.google.com/file/d/1zkpNgoUz8kTdER5dA2YcrfJV9dT_R74I/view?usp=sharing) ulaşabilirsiniz.

## Lojistik Hatırlatmalar
Final Projesi programı bitirme oranınızda önemli bir yere sahiptir.
Projede size verilen başlangıç kodlarında belli değişkenler ve fonksiyon önerileri tanımlanmıştır, bunları kullanabileceğiniz 
gibi kendi fonksiyonlarınızı da yazabilirsiniz.

Final Projesi 3 ana aşamaya ayrılmıştır, bu aşamaların açıklamalarını aşağıda bulabilirsiniz.   
<span>1.</span> Aşamanın teslim tarihi **8 Aralık Çarşamba**,   
<span>2.</span> Aşamanın teslim tarihi: **22 Aralık Çarşamba** 
<span>3.</span> Aşamanın teslim tarihi: **2 Ocak Pazar** olarak belirlenmiştir. 

Bonus ile belirtilen görevler zorunlu değildir, sadece oyununuzu geliştirebilecek önerilerdir. Yaratıcılığınızı
kullanıp ek özellikler ekleyebilirsiniz, hatta bunları Ed'den hepimizle paylaşın!

### Aşamalar
#### 1. Aşama
- Oyun Arka Planı
    - Yolun çizilmesi
    - Ağaçların çizilmesi
    - Arabaların çizilmesi
- Oyun Döngüsü
    - Ağaçların hareketinin sağlanması

Dokümantasyonun uzun olmasından korkmayın &#128519; bu sayfada final projesini yazarken
ihtiyaç duyabileceğiniz bütün bilgileri kapsamaya ve görevlerinizi elimizden 
geldiğince detaylı açıklamaya çalıştık.

Her ödevimizde olduğu gibi Final Projesinde de arkadaşlarınızla sözlü olarak fikir alışverişinde
bulunabilirsiniz. Ancak akademik dürüstlük ilkelerini doğrultusunda kod değiş tokuşu yasaktır ve ödevinizin geçersiz sayılmasına neden olabilir.

Başarılar &#128640;!

##  Hikaye

Bir gün arkadaşınızla sokakta gezinirken arkadaşınız sizden çok daha iyi oyun oynadığını iddia etti.
Siz de oyunlarda daha iyi olduğunuzu kanıtlayabilmek için oyuncuların sırayla oynadığı bir araba yarışı oyunu hazırlamaya karar verdiniz.
Bu oyunda kazandığınız puanları karşılaştırarak arkadaşınızdan daha iyi olduğunuzu gösterebilirsiniz!

##  1. Aşama

1. Arabayı sürebileceğiniz bir alan olarak bir `Canvas` oluşturun.

- Kanvasın boyutları başlangıç kodunda `KANVAS_EN` ve `KANVAS_BOY` değişkenleriyle verilmiştir.

- Kanvasın başlığını "Final Projesi" olarak ayarlayın.

2. Yol çizgilerini oluşturacak fonksyionu yazın.

- Bu fonksiyonu yazarken ortadaki çizginin kanvasın tam ortasından geçmesine ve yol genişliklerine dikkkat edin. Her şerit `KANVAS_EN`in çeyregi genişlikte olmalı.
- Yolun genişligi olarak size verilen `YOL_EN` degişkenini kullanabilirsiniz, unutmayın ki bu iki şeritli yolun toplan genişligi olmalı.

3. Arabaları oluşturacak kodları yazın

- Arabaları çizdirirken başlangıç kodunda size verilmiş olan pozisyon ve boy değişkenlerini kullanabilirsiniz.
- Projenin bu aşamasında arabaların hareket etmesi gerekmiyor, çalışmalarınızı ona göre yapabilirsiniz.

4. Ağaçları oluşturacak kodu yazın

- Bunun için `soldaki_agacları_olustur` ve `sagdaki_agacları_olustur` olmak üzere iki fonksiyon doldurmalısınız. Bu fonksiyonlar neredeyse aynı görevi yapacak, ancak bir tanesi ekranın sag tarafindaki digeri ise sol tarafindaki agacların çizilmesi için. 
- Bu fonksiyonlar her çagırıldıgında ekranın ilgili kısmında ve en üstte birer tane agaç yaratmalı. Agaçların yaratılacagı x koordinatları rastgele bir şekilde seçilmeli. Degerleri belirlerken `SOL_AGAC_MIN` `SOL_AGAC_MAX` `SAG_AGAC_MIN` ve `SAG_AGAC_MAX` degişkenlerinden faydalanabilirsiniz.
- İki sayı arasında rastgele bir sayı seçmek için `random.randint(MIN, MAX)` fonksiyonunu kullanabilirsiniz. (MIN sayının alabilecegi en küçük degeri, MAX ise en büyük degeri içermeli)
- Ağaçları çizdirirken başlangıç kodunda size verilmiş olan pozisyon ve boy değişkenlerini kullanabilirsiniz.

5. Her adımda ağaçları hareket ettiricek ve ekran dışına çıkacak olan ağaçları silecek kodu yazın

- Agaçlar oluşturulduktan sonra ilk aşamada `MIN_BASLANGIC_HIZ` hızıyla aşagı dogru hareket etmeli, böylece animasyonumuzda arabalar ilerliyor gibi gözükecek ve oyunumuzun arka planını tamamlamış olacagız.
- Bu aşamada ekranın dışına çıkan agaçları silmeyi unutmamalıyız!!! Yoksa oyunumuz bir süre sonra bütün agaçları hareket ettirmeye çalışmaktan yorulup yavaşlayacaktır ve kimse böyle bir oyun oynamak istemez :)
- Agaçların hareket ettirilmesi ve ekran dışına çıkan araçların silinmesi konusunda daha önce grup çalışmalarında yaptığımız yağmur damlası simülasyonlarından yardım alablirsiniz.

**Not:** Pythonda stringlerin içerisinde Türkçe karakterleri kullanabildiğimiz gibi tüm dünya dillerinin karakterlerini, hatta emojileri bile kullanabilirsiniz. Tüm emojilerin listesine [buradan](https://unicode.org/emoji/charts/emoji-list.html) ulaşabilirsin.

```python
>>> print("\u2764\ufe0f")
❤️
```


Bu adımlar tamamlandıktan sonra Aşama 1'in sonucu olarak aşağıdaki gibi bir görüntü elde edilmeli. Unutmayın yeşil noktalar haraket ediyor olacak.

![Ana Ekran](/assets/images/2021fall/final_project/asama1.png){: width="450px" }
    
