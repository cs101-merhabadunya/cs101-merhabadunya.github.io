---
layout: post
title: Hafta 7 - Grup Çalışması Egzersizleri
subtitle: Dict ve Kanvas
categories: grup çalışması
authors: [Ece Pınar Özer, Arda Rutkay Var]
tags: [grup çalışması]
slug: hafta7-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/drive/folders/1P0nSHGlAeK6pS2pjgtNL6B_rEFz8itQU) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1

Bir kahveci süt, krema, sos ve aroma kullanarak kahveler hazırlamaktadır.
Kahveci bu ürünlerden birisi tükendiği takdirde yeni gelen müşterilerine
ürün yok dememek için kahve satışını kapatmaktadır.
Ayrıca kahveci, eklenilen ürünlere göre kahvenin kaç kalori tuttuğunu da
söylemek istemektedir.

Yalnızca bir çeşit ürün kahveye eklenebilmektedir.

Biz de kahvecinin deposundaki ürünleri ve onların kalori değerlerini
bir sözlükte tutarak gelen müşterilere bunları birer seçenek olarak sunacağız.

`malzeme_var_mı(dict)` ile ürün olup olmadığını kontrol etmek istiyoruz.
`depodaki_urunleri_goster(dict)` ile ürünleri müşteriye göstermek istiyoruz.

Ürün satıldığında ürünlerimizin sayısını güncellememiz ve müşteriye
kahvesinin kaç kalori tuttuğunu söylememiz gerek.
Herhangi bir ürün tamamen bittiğinde de kahve satışı bitecek.



```
Örnek Çalışma Biçimi #1:
Elimizdeki ürünler: 
Krema -> 20 birim
Süt -> 30 birim
Sos -> 20 birim
Aroma -> 25 birim
> Hangi ürünleri ekletmek istersiniz? Krema
> Kaç birim istersiniz? 25
Elimizde 25 birim Krema yok. Size 20 Krema ekleyebileceğim.
Kahveniz toplam: 5000 kalori.
Kahve satışı bitti.



Örnek Çalışma Biçimi #2
Elimizdeki ürünler: 
Krema -> 20 birim
Süt -> 30 birim
Sos -> 20 birim
Aroma -> 25 birim
> Hangi ürünleri ekletmek istersiniz? Karamel
Biz Karamel satmıyoruz.
Elimizdeki ürünler: 
Krema -> 20 birim
Süt -> 30 birim
Sos -> 20 birim
Aroma -> 25 birim
> Hangi ürünleri ekletmek istersiniz? Süt
> Kaç birim istersiniz? 30
Kahveniz toplam: 3000 kalori.
Kahve satışı bitti.
```

## Egzersiz 2

Beraber oyun oynarlarken Dory, Nemo'yu kaybetmiştir. Kafası karışan ve kalabalık içinde Nemo'yu bulamayan Dory,
olduğu yerde Nemo'ya seslenmekte, Nemo'nun kendisini bulmasını beklemektedir. Kanvas üzerinde, 20 adet Nemo olmayan
sarı balık ve Nemo'yu rastgele hızlarla, rastgele yönlere doğru hareket ettirmeli, herhangi bir kenara çarptığında
sekerek ekranda kalmaya devam etmelerini sağlamalıyız. Nemo, Dory'yi bulduğunda hareketi durdurup, Dory'ye müjdeyi vermeliyiz!

Dory haricindeki her balık sözlük içerisinde key olarak depo edilmeli. Her bir balık için 3 elemanlı bir liste, (```hiz_x```, ```hiz_y``` ve Nemo mu değil mi bilgisini içeren (```True```/```False```)), value olarak saklanmalı.

Nemo, Dory'nin yanına geldiğinde simulasyon durmalı. Canvas sınıfına ait, ```find_overlapping()``` fonksiyonu oldukça iş görebilir.

[Buraya tıklayarak](https://drive.google.com/file/d/1eHOyyIUYlu4EdG3CVGmVOn-RFPeHgqVF/view?usp=sharing) programın nasıl çalışması gerektiğini görebilirsiniz.

<video src="https://drive.google.com/file/d/1eHOyyIUYlu4EdG3CVGmVOn-RFPeHgqVF/preview" width="640" height="480"></iframe>

Önce Sözlük tanımlayarak başlayabiliriz. ```balıklar = {}```

ÖRNEK:
```balık = {balık1:[hiz_x, hiz_y, False], balık2:[hiz_x, hiz_y, False], ... balık20:[hiz_x, hiz_y, False], nemo:[hiz_x, hiz_y, True]}```

AŞAMA 1 - Balık ekleme:
```create_image_with_size()``` fonksiyonu ile ekranda istenilen bölgeye bir balık eklenebilir. Burada görsel olarak resimler klasörü altında verilen ```balık.jpg``` kullanılmalı.
```random``` kütüphanesini kullanarak iki farklı sayı seçip hız değerleri şeklinde kaydedip, sözlüğe ilgili şekilde ekleyebiliriz.
Bu aşamadaki balıklar Nemo olmadığı için sözlüğe False değerini eklemeyi unutmayalım. 

AŞAMA 2 - Hareket ettirme:
Hareket ettirme (```hareket_ettir(balıklar)```) fonksiyonu sürekli çalışmalı, mesela bir döngünün içinde olması çok iyi olur. Ve döngü her döndüğünde 1 saniye durduğunu varsayın. Bu bir saniyede dictionary içerisindeki her balık için ```find_overlapping()``` fonksiyonunu kullanarak Nemo'nun Dory ile kesişip kesişmediğini görebiliriz değil mi? (```nemo_geldi()```)

AŞAMA 3 - Nemo'nun Dory'nin yanına gelişi:
```nemo_geldi()```fonksiyonu Dory ile kesişimi bulunan balıklar içinde Nemo varsa True değeri döndürmeli.

AŞAMA 4 - Bitirme:
Eğer Nemo Dory'nin yanına geldiyse programı durdurmalıyız.


## Bonus

### Egzersiz 1

ROT Şifreleyici ve Şifre Çözücü

ROT şifreleme tekniği en çok bilinen ve en basit şifreleme methodlarından bir tanesidir.
Basit olarak alfabedeki her bir harfi belirli sayıda ilerideki harfe atama prensibinden oluşur.

Sizden istediğimiz öncelikle kullanıcıya
şifreleme mi şifreyi çözme mi yapmak istediğini sormanız.
Kullanıcı E basarsa şifreleme, D basarsa deşifreleme, başka bir şey basarsa tekrar isteme işlemleri uygulanmalı.

Daha sonra tercihe göre dictionary veri tipi kullanarak alfabedeki her bir harfi kullanıcıdan
alacağınız sayı kadar sonraki veya önceki harfe atamanız
ve sonucu şifreleme için encode() ve deşifreleme için decode() fonksiyonlarını
kullanarak ekrana bastırmanız.

Örnek Çalışma:
```
> Şifreleme için E'ye, deşifre için D'ye basınız: E
> Rotate sayısını girin: 7
> Şifrelenecek mesajı küçük harflerle girin: merhaba dünya
```
Programın çıktısı aşağıdaki gibi olmalı:
```
{'a': 'g', 'b': 'ğ', 'c': 'h', 'ç': 'ı', 'd': 'i', 'e': 'j', 'f': 'k', 'g': 'l', 'ğ': 'm', 'h': 'n', 'ı': 'o', 'i': 'ö', 'j': 'p', 'k': 'r', 'l': 's', 'm': 'ş', 'n': 't', 'o': 'u', 'ö': 'ü', 'p': 'v', 'r': 'y', 's': 'z', 'ş': 'a', 't': 'b', 'u': 'c', 'ü': 'ç', 'v': 'd', 'y': 'e', 'z': 'f'}

şjyngğg
içteg
Program Bitti
```