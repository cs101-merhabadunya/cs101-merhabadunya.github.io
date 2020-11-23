---
layout: post
title: Hafta 4 - Grup Çalışması Egzersizleri
subtitle: While Döngüsü ve Grafik Kütüphanesi
categories: grup çalışması
authors: [Demet Tümkaya, Fırat Tamur]
tags: [grup çalışması]
slug: hafta4-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/file/d/13x2Z3ttEKilyAclRVVw6n7eceDGj-o50/view?usp=sharing) bu haftaya ait çalışmaların başlangıç kodlarına ve oyundaki araba resimlerine ulaşabilirsiniz.

## Egzersiz 1

Kasiyer Selin Hanım müşterilerin aldıkları ürünlerin fiyatlarının toplamını bulmak istiyor. Ona yardımcı olmak için bir program hazırlayalım. Selin Hanım girdi olarak 0 girene kadar ürünlerin fiyatları toplanmaya devam etmelidir.

```
# Örnek Çalışma Şekli

Merhabalar, toplam fiyatı öğrenmek için fiyatları girmeye başlayabilirsiniz!
> Ürün fiyatı giriniz: 5
> Ürün fiyatı giriniz: 10
> Ürün fiyatı giriniz: 14.5
> Ürün fiyatı giriniz: 3.75
> Ürün fiyatı giriniz: 0
Toplam fiyat: 33.25

```

![](https://images.pexels.com/photos/3907161/pexels-photo-3907161.jpeg?cs=srgb&dl=pexels-andrea-piacquadio-3907161.jpg&fm=jpg)

## Araba Oyunu

Bu egzersizde Python’da Grafik kütüphanesini ve while döngülerini kullanarak 4. dersimizde gördüğümüz oyunu geliştirmeye başlayacağız. Oyunun bu haftaki aşamasında hedeflerimiz:
- Ekrana bir yazı (text) ekleyerek kullanıcıya fareyle ekrana tıkladığında oyunu başlatabileceğini bildirmek.
- Kanvasımızın üzerine yolun şeritlerini çizdirmek.
- Yeşil ve mavi araçların kanvas üzerindeki pozisyonlarını verilen sabitleri kullanarak belirlemek ve basit dikdörtgenler olarak yoldaki şeritlere eklemek. Araçlar şeritlerinin tam ortasında olmalı.
- Araçları sürekli aşağı doğru hareket ettirmek.
- Ekrandan çıkan araçların tekrar başlangıç pozisyonlarından rastgele yeni bir hızla hareket etmesini sağlamak. Ancak araçlar ekrandan çıktıktan sonra yeni bir hız belirlemelisiniz.
### Oyununuza isterseniz ekleyebileceğiniz bonus özellikler:
- Araçları çizmekte kullandığınız dikdörtgenleri başlangıç kodunda verilen resimlerle değiştirmek
- Daha fazla şerit ve araç eklemek
- Skor eklemek (arabaların kaç kere yolu tamamladığı üzerine iki skor tanımlayabilirsiniz)
## Oyun Videosu
 Bu haftaki hedeflerimiz bittiğinde oyunumuzun nasıl görüneceğini aşağıdaki videodan izleyebilirsiniz:
<iframe src="https://drive.google.com/file/d/14-YbEiv2qRbv0HwvfLZovXMkT_bUxMds/preview" width="640" height="480" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
[Buraya tıklayarak](https://drive.google.com/file/d/1Z0V48Gl_6YYi195LPJJorN54yS1gZmwn/view?usp=sharing) oyunumuzun tamamlandığında nasıl görüneceğini izleyebilirsiniz.
## Oyun Tasarımı
<!-- <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vS9DXKtrTWnZI4Z0yHsExtX7jlPuWO7IR7lhK5HWuGD4jmeFfBpx99hWGI81lM6Ezf6NYemvMyHusam/embed?start=false&loop=true&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe> -->
Grafik programları yazarken ortaya çıkarmak istediğimiz programı canlandırmak her zaman ilk aşama olmalı, bu sayede koordinatları, objelerin birbirleriyle ilişkilerini kolayca anlayabiliriz. İlk grafik programımızda bu konuda size biraz yardımcı olmak istedik, aşağıda kanvasımızın genel görüntüsünü bulabilirsiniz.

![](https://drive.google.com/file/d/147McyCDVvJs7XoopZOAnUd5p4w9sNxw_/view?usp=sharing)
Elle çizildiği için bazı küçük kaymalar olabilir ancak zaten bu taslağı sadece bize yardımcı olması için çiziyoruz, mükemmel olmak zorunda değil :).

## Ekstra Egzersizler

### Egzersiz 1

Özellikle şu zamanlarda zamanı kontrol etmek çoğumuz için zor oluyor. Sevdiğimiz şeyler üzerinde daha çok zaman harcamayı tercih ederken sorumluluklarımızı da aksatmamaya çalışıyoruz. Bize bir şey üzerinde yeterince uğraştığımızı verdiğimiz süre içerisinde geriye doğru sayarak ve bittiğinde de bildiren bir program yazalım.

Not: Programın her bir saniyede çalışması için time kütüphanesini projeye dahil etmeyi ve time.sleep(saniye) fonksiyonunu kullanmayı unutma! Bu fonksiyon programın "saniye" kısmına girdiğiniz süre kadar beklemesini sağlar.

```
# Örnek Çalışma Şekli

> Seni süre bittiğinde uyarmam için kaç saniye geçmeli? 360
Süre başlıyor...
360
359
...
...
...
1
0
Süren bitti!

```

![](https://images.pexels.com/photos/1178684/pexels-photo-1178684.jpeg?cs=srgb&dl=pexels-mike-1178684.jpg&fm=jpg)

### Egzersiz 2

1 den büyük asal olmayan bir tamsayının rakamlarının toplamı, sayının çarpanlarına ayrılarak yazıldığında, bu yazılışta bulunan tüm asal sayıların rakamlarının toplamına eşitse bu sayı bir Smith sayısıdır. 
Örneğin, 728 sayısı asal çarpanlarına 728 = 2 . 2 . 2 . 7 . 13 biçiminde ayrılır. 7 + 2 + 8 = 17 = 2 + 2 + 2 + 7 + (1 + 3) olduğundan 728 bir Smith sayısıdır.
Bu egzersizde kullanıcı negatif bir sayı girene kadar ondan sayılar girip bu sayıların Smith sayısı olup olmadığını konsola yazdırmalısın.

```
# Örnek Çalışma Şekli

> Bir sayı gir: 2
2 bir Smith sayısı değil
> Bir sayı gir: 3
3 bir Smith sayısı değil
> Bir sayı gir: 4
4 bir Smith sayısı
> Bir sayı gir: 5
5 bir Smith sayısı değil
> Bir sayı gir: 4937775
4937775 bir Smith sayısı
> Bir sayı gir: -1
Görüşmek üzere

```

![](https://images.pexels.com/photos/1364700/pexels-photo-1364700.jpeg?cs=srgb&dl=pexels-logan-kirschner-1364700.jpg&fm=jpg)
