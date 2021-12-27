---
layout: post
title: Final Projesi
subtitle: 
categories: final_projesi
authors: [Yağmur Akarken, Ece Pınar Özer, İdil Defne Çekin, Burak Aslantaş,Ceren Kocaoğullar, Burcu Yıldız ]
tags: [final_projesi]
slug: final-projesi

---


| # Aşama  |             Yazarlar             |
| :------: | :------------------------------: |
| 1. Aşama |  Yağmur Akarken, Ece Pınar Özer  |
| 2. Aşama | İdil Defne Çekin, Burak Aslantaş |
| 3. Aşama | Ceren Kocaoğullar, Burcu Yıldız  |



CS 101 Güz 2021'in 6 haftasını geride bıraktık! Şimdiye kadar inanılmaz bir gelişme gösterdiğiniz ve 
programı takip ettiğiniz için hepinizi tebrik ederiz. Programın son 2 haftasında Final Projesi yaparak 
öğrendiklerinizi bir oyunla ölümsüzleştireceksiniz. 

Aşağıda Final Projesi ile ilgili verilen açıklamayı lütfen dikkatlice okuyun, başarılar.

## Başlangıç Kodları
Final Projesine ait başlangıç kodlarına [buradan `(Gitmek için tıkla)`](https://drive.google.com/file/d/1zkpNgoUz8kTdER5dA2YcrfJV9dT_R74I) ulaşabilirsiniz.

İkinci aşamanın başlangıç kodlarına [buradan `(Gitmek için tıkla)`](https://drive.google.com/file/d/1yd4lv1xmlkjVkZl9xdTBLGq_80mbQB7v/view?usp=sharing) ulaşabilirsiniz. 

Başlangıç kodları ilk aşamada yaptıgınız aşamaların çözümlerini de içeriyor, yani ilk aşamayı tamamlayamadıysanız veya eksikleriniz varsa da ikinci aşamadan projeye devam edebilirsiniz :)!!! Ayrıca bizim verdigimiz çözümler yerine dilerseniz kendi yazdıgınız fonksiyonları da kullanabilirsiniz. Yaratıcılıgınızı kullanmaktan çekinmeyin, oyununuzu kendinize göre modifiye edebilirsiniz :) 

## Lojistik Hatırlatmalar
Final Projesi programı bitirme oranınızda önemli bir yere sahiptir.
Projede size verilen başlangıç kodlarında belli değişkenler ve fonksiyon önerileri tanımlanmıştır, bunları kullanabileceğiniz 
gibi kendi fonksiyonlarınızı da yazabilirsiniz.

Final Projesi 2 ana aşamaya ayrılmıştır, bu aşamaların açıklamalarını aşağıda bulabilirsiniz.   
<span>1.</span> Aşamanın teslim tarihi **8 Aralık Çarşamba**,   
<span>2.</span> Aşamanın teslim tarihi **22 Aralık Çarşamba**,   
<span>3.</span> Aşamanın teslim tarihi: **2 Ocak Pazar** olarak belirlenmiştir.  
Her aşamanın sonunda, ilgili aşamanın çözümlerini sizinle paylaşacağız. Bu çözümleri sonraki aşamaları kodlarken kullanabilirsiniz. Böylece bir aşamada takıldığınızda, diğer aşamayı çözebileceksiniz.
Bonus ile belirtilen görevler zorunlu değildir, sadece oyununuzu geliştirebilecek önerilerdir. Yaratıcılığınızı
kullanıp ek özellikler ekleyebilirsiniz, hatta bunları Ed'den hepimizle paylaşın!

### Aşamalar
#### 1. Aşama
- Oyun Arka Planı
    - Arabayı oluştur
    - Arabanın gideceği yolları oluştur
    - Yol kenarlarında yeşil ağaçlar (yeşil daireler) oluştur
- Oyun Döngüsü
    - Konsoldan arabanın rengini girdi (input) olarak al
    - Yol kenarlarında oluşturulan yeşil ağaçları, yukarıdan aşağıya doğru hareket ettir. (İpucu: Haftalık verilen ödevlerdeki "Yağmur yağdırma" örneğinden esinlenebilirsin.)
#### 2. Aşama
- Yön tuşlarıyla arabayı hareket ettir (Yön tuşları klavyenizde bulunan bu tuşlardır, "`←`, `↑`, `→`, `↓`")
- Yol üzerinde rastgele engel oluştur
- Çarpışmaları kontrol et (Kodunuzu **kütüphane kullanmadan** oluşturun)
    - Eğer çarpışma gerçekleştiyse, oyunu durdur
- Engelleri hareket ettir
#### 3. Aşama
- Birden fazla oyuncuya sırayla oynatın
- Skor tutun
- Can kontrolü
    - Eğer canlar bittiyse, sonraki oyuncuya geçin
    
Dokümantasyonun uzun olmasından korkmayın &#128519; bu sayfada final projesini yazarken
ihtiyaç duyabileceğiniz bütün bilgileri kapsamaya ve görevlerinizi elimizden 
geldiğince detaylı açıklamaya çalıştık.

Her ödevimizde olduğu gibi Final Projesinde de arkadaşlarınızla sözlü olarak fikir alışverişinde
bulunabilirsiniz. Ancak akademik dürüstlük ilkelerini doğrultusunda kod değiş tokuşu yasaktır ve ödevinizin geçersiz sayılmasına neden olabilir. Tüm sorularınızı [Ed `(Gitmek için tıkla)` ](https://edstem.org/us/courses/15472/discussion/904782)
sayfamızdan eğitmenlerinize sorabilirsiniz.

Başarılar &#128640;!
### Ön Hazırlık
Grafik kütüphanemizi kullanarak resim eklemek ya da resimler üzerinde değişiklik yapmak 
için Pillow isimli ek bir paket indirmemiz gerek. Pillow'u indirmek için bir terminal 
penceresi açın (PyCharm'ın içindeki Terminal sekmesini kullanabilirsiniz) ve aşağıdaki 
komutu girin:  
Windows için:
```bash
python -m pip install Pillow==7.1.1
``` 
Mac için:
```bash
python3 -m pip install Pillow==7.1.1
```

Kurulum başarı ile tamamlandığında terminalinizde son olarak "Successfully installed Pillow-7.1.1" ibaresi görünür. Artık grafik kütüphanemizdeki resim içeren fonksiyonları kullanabiliriz!

## Hikaye
Bir gün arkadaşınızla sokakta gezinirken arkadaşınız sizden çok daha iyi oyun oynadığını iddia etti. Siz de oyunlarda daha iyi olduğunuzu kanıtlayabilmek için oyuncuların sırayla oynadığı bir araba yarışı oyunu hazırlamaya karar verdiniz. Bu oyunda kazandığınız puanları karşılaştırarak arkadaşınızdan daha iyi olduğunuzu gösterebilirsiniz!

## 1. Aşama

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

## 2. Aşama
### 2.A Arabayı hareket ettir
Arabayı yön tuşlarıyla hareket ettirelim. (Yön tuşları klavyenizde bulunan bu tuşlardır, "`←`, `↑`, `→`, `↓`")

- Başlangıç kodlarında verilen `arabayi_hareket_ettir` fonksiyonunu yazın. Bu fonksiyon
parametre olarak oyun `kanvas`ını ve `araba` objesini alır.  
**İpucu:** Yön tuşlarını kullanarak bir objeyi hareket ettirmek için Hafta 6 Grup Çalışması egzersizlerinde yaptıgımız yemleri yiyen topçuk
örnegini inceleyebilirsiniz. Hatırlarsanız burada hangi tuşa basıldıgını kontrol etmek için `kanvas.get_new_key_presses()` fonksiyonunu ve tuşu ayırt etmek için ise tuşların sym kodlarını kullanmıştık. Ok tuşlarının kodları sırasıyla (`Left`, `Up`, `Right`, `Down`)
**İpucu:** Kanvasta bir objenin mutlak konumunu değiştirmek için `kanvas.move(obje, dx, dy)`
fonksiyonunu kullanabilirsiniz.
- Oyunu çalıştırırken fark edeceksiniz ki bu haliyle araba 
kanvasın dışına da çıkabilir. Bunu engellemek için karakterin konumunu güncellerken 
ilerleyebileceği maksimum ve minimum koordinatları kontrol edebilirsiniz.

 ### 2.B Rastgele engel oluşturulması
 Artık engelleri kanvasa ekleyebilirsiniz.
 1. Engelleri kanvasa dikdörtgen olarak ekleyeceksiniz. 
 2. Engelleri eklemek için `rastgele_engel_olustur(kanvas, engel_listesi)`
 fonksiyonunu yazın. Bu fonksiyon her çalıştığında %20 ihtimalle engel oluşturur ve engel listesine ekler. Bir işlemin %20 ihtimalle yapılmasını saglayan kodu fonksiyonun içerisinde hazır olarak size verdik, başlangıç kodlarını incelemeyi unutmayın! Burada dikdörtgenler oluşturalım. Dikdörtgenlerin boyutu, `ENGEL_EN` x `ENGEL_BOY` olmalı. Son olarak dikdörtgenlerin rengi kahverengi olmalı, canvas kütüphanesini kullanarak `kanvas.COLORS.Brown4` ile kahverengini elde edebilirsiniz. Kolaylık olması açısından `ENGEL_EN` ve `ENGEL_BOY` kodun başında sabit olarak tanımlanmıştır.  

### 2.C Çarpışmalar &#x2607;

 - Animasyonunuzun her aşamasında arabanın yoldaki engellerle çarpışıp çarpışmadığını 
 kontrol etmelisiniz. Bunun için başlangıç kodlarında `carpismalari_kontrol_et(kanvas, araba, engel_listesi)`
 olarak verilen fonksiyonu yazın. Bu fonksiyonda `kanvas.find_overlapping` fonksiyonunu
 kullanarak kanvas üzerinde ana karakterle çakışan konumdaki objeleri bulabilirsiniz.   
 **İpucu 1:** `kanvas.find_overlapping` x1, y1, x2, y2 olmak üzere 4 argüman alır ve 
 kanvasta arabanın bulunduğu karenin koordinatlarını kullanabilirsiniz.  
 **İpucu 2:** `kanvas.find_overlapping` bir liste döndürür. Bu listedeki her elemanın "engel"
 olup olmadığını nasıl anlayabilirsiniz? `engel_listesi`'nden faydalanabilirsiniz! 
 **İpucu 3:** Çarpışma gerçekleştiğinde, oyunu durdurmak için `kanvas.wait_for_click()` fonksiyonunu hatırlayın.
 
 ### 2.D Engelleri hareket ettir
 Artık engelleri hareket ettirebilirsiniz. Bunun için, 
 1. Engelleri hareket ettir. Animasyonun akan bir yol gibi gözükmesi için engellerin agaçlarla aynı hızda hareket etmesi gerekiyor. 
 2. Kanvasın dışına çıkan engelleri kanvastan sil,
 İpucu: Ağaçları hareket ettirip, kanvas dışına çıktığına silme işlemini yapan, benzer bir fonksiyonu, başlangıç kodunda bulabilirsiniz.

## 3. Aşama
Bu aşamada birden fazla oyuncunun sırayla oynamasını sağlayacaksınız. Oyuncular canı bitene kadar devam edebilecek. Skor tutacaksınız. Tüm oyuncular oynamayı bitirdiğinde de skorları ve kazananı konsola yazdıracaksınız.
Adım adım yapmanız gerekenler şu şekilde:
1. 'oyunculari_al()' metodunu şu şekilde doldurun: Konsol aracılığıyla kaç oyuncu oynayacağını sorun. Her bir oyuncu için oyuncunun ismini konsoldan alın. 
2.  Tüm oyunun her bir oyuncu için tekrarlanması gerekiyor. 
(İpucu 1: Elinizde 'oyuncu_adlari' listesinin olduğunu unutmayın.)
(İpucu 2: Oyunun başladığı ve bittiği yerleri sizin için kodda gösterdik.)
(İpucu 3: Birden fazla satırı aynı anda seçip klavyenizin TAB tuşuna basarsanız, satırların hepsi bir basamak içeri kayar.)
3. Oyuncular kaçmayı başardıkları (yani çarpışmadan ekrandan silinen) her engel için bir puan kazanmalı.
4. Oyuncu bir engelden kaçmayı başaramaz ve çarparsa canı azalmalı. ('carpisma_kontrol_et' metodunu sizin için düzenledik; çarpıştığı engeller yok olacak.)
5. Bilgi göstergesini yeni skor ve canla güncellemelisiniz.
(İpucu 1: Son grup çalışmasında kullandığımız 'set_text' metodu işinize yarayabilir.)
(İpucu 2: Ekrana yazdırmanız gereken format için 'create_text' metodunu nasıl çağırdığımızdan kopya çekebilirsiniz.)
6. Can bittiğinde o oyuncu için oyunu bitirmeyi unutmayın. 
(İpucu: 'break' işinizi görebilir.)
7. Oyun bittiğinde konsola yazabilmek için skorları bir sözlükte tutun.
8. 'sonuclari_yazdir' metodunu şu şekilde doldurup, herkes için oyun bittikten sonra çağırın: Her bir oyuncunun skorunu ve en çok skoru alan oyuncunun adını konsola yazdırın. 

<iframe width="560" height="315" src="https://drive.google.com/file/d/17p2HKexjNJWkiE4E1l2PchjQuvWhQJm5/view?usp=sharing" title="Final Projesi Kaydı" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
