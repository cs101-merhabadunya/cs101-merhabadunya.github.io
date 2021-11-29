---
layout: post
title: Hafta 6 - Grup Çalışması Egzersizleri
subtitle: Klavye ve mouse olayları
categories: grup çalışması
authors: [İdil Defne Çekin, Burak Aslantaş]
tags: [grup çalışması]
slug: hafta6-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/drive/folders/1ziMqXDv_8H3tejXtFtsr3zgLnTdZpemv?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1
Grup liderlerimiz farklı oranlarda ve büyüklüklerde oval şekilleri kullanarak
elektronik sanat eserleri oluşturmak istiyorlar, bu konuda onlara yardımcı
olacak bir program yazalım.

Sanat eserimizi 800'e 600 birimlik siyah bir kanvas üzerine mause'la tıkladığımız
yerleri merkez olarak alan, rastgele renklerde ovaller çizerek oluşturacağız. Eserimizde
geometrinin gücünü kullanmak için çizdiğimiz ovallerin eninin mouse'la tıkladığımız x
koordinatının yarısı, boyununsa mouse'la tıkladığımız y koordinatının yarısı kadar olmasını
istiyoruz. Ovallerin renklerini rastgele seçmek için hazır olarak verilen `rastgele_renk_sec()`
fonksiyonunu kullanabiliriz.

### Tamamlamamız gereken adımlar:
1. Kanvasın arkaplan rengini siyah yapmak (Black).
2. Kanvasın mausea basıldığında `oval_ciz` fonksiyonunu cağırmasını ve güncellenerek
yeni değişiklikleri göstermesini sağlamak.
3. `oval_ciz` fonksiyonunu doldurmak.

Örnek bir sanat eseri aşagıdaki gibi olacaktır:

<img align="center" src="https://github.com/cs101-merhabadunya/cs101-code/raw/master/guz2021/sections/hafta6/hafta6_egzersiz1_baslangic.jpeg" 
     width="600" 
     height="450" />

## Egzersiz 2
Bu egzersizde 2000'lerin klasik oyunu Snake (Yılan) gibi bir oyun yazacağız. Yem ve top oluşturan
fonksiyonları başlangıç kodunda verdik. 
`yem_olustur` kanvasta rastgele bir konumda yem (kırmızı bir oval) oluşturur.
- `topu_olustur` kanvasın tam ortasında mavi bir top oluşturur.  
Sizin göreviniz animasyon boyunca kullanıcının klavye hareketlerini kontrol ederek 
topun basılan tuş yönünde hareket etmesini sağlamak.
' 'yem_olustur` fonksiyonunu kullanarak `YEM_SAYISI` kadar yem oluşturun. Unutmayın
oluşturduğunuz yemleri ileride kullanacaksınız.
- `topu_hareket_ettir(kanvas, top)` fonksiyonunda `kanvas.get_new_key_presses()` kullanarak
topu `TOP_HIZ` birim kadar hareket ettirin. `w` yukarı, `a` sol, `s` aşağı ve `d` de sağ yönde hareketi temsil eder.  
- Topun yediği yemleri bulun ve ekrandan kaldırın.  
**ipucu:** `kanvas.find_overlapping` fonksiyonunu kullanabilirsiniz.
- Tüm yemler bittiğinde kanvastaki bütün objeleri kaldırın ve tebrik mesajı görüntüleyin.


Egzersizin bitmiş hali tek yem ile aşağıdaki videodaki gibi çalışmalı:

<iframe src="https://drive.google.com/file/d/1Di-dwQ61ioDP_KhLWwUp6tYgVVTLz4h6/preview" width="640" height="480">allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

[Buraya tıklayarak](https://drive.google.com/file/d/1Di-dwQ61ioDP_KhLWwUp6tYgVVTLz4h6/view?usp=sharing) egzersizin tamamlandığında nasıl görüneceğini izleyebilirsiniz.

## Ekstra 1

Burak, bebek kardeşini eğlendirmek için bir kod yazmak istiyor. İyice düşündükten
sonra kardeşini en çok eğlendiren oyuncaklarının hep bir tuşa basıldığında
renkler çıkaran oyuncaklar olduğunu fark ediyor. Kardeşinin ismi de Gökçen olduğu için baş
harfi olan G'ye basıldığında kanvasa renkli bir şekil koyan bir kod yazmaya karar veriyor.

Hadi Burak'a yardımcı olalım.
### Tamamlamamız gereken adımlar:

Bu alıştırmada grafik kütüphanesini kullanarak kanvas üzerine;
 1. Rastgele renkte ve yerde OVAL çıkaran,
 2. Rastgele renkte ve yerde DIKDORTGEN çıkaran bir kod yazacağız.
Bunun için aşağıda açıklamaları verilen dört fonksiyonu kullanmamız gerek.
`rastgele_renk_sec()` fonksiyonunu sizin için önceden tanımladık. Sizin göreviniz `topcuk_yarat(renk)`,
`kutucuk_yarat(renk)` ve `rastgele_topcuk_cikar(key)` fonksiyonlarını tanımlamak
tabii ki son adımda görevimizi `main()`'in içinde tamamlamayı unutmayın!
**ipucu:** Bu egzersizde grafik kütüphanesinde yer alan `set_on_key_pressed` fonksiyonunu
kullanabiliriz.
