---
layout: post
title: Hafta 4 - Grup Çalışması Egzersizleri
subtitle: While Döngüsü ve Grafik Kütüphanesi
categories: grup çalışması
authors: [Demet Tümkaya, Fırat Tamur]
tags: [grup çalışması]
slug: hafta4-grup
---

Geçen hafta cumartesi dersimizde while döngüleri ve grafik kütüphanesini işledik. While döngülerinin oyunlarda sık kullanıldığını öğrendik. Bu yüzden hem while döngülerini anlamak hem de grafik kütüphanesinin bize sağladığı fonksiyonları öğrenmek için basit bir oyun tasarladık. Oyunun videosunu aşağıda bulabilirsiniz. Oyunu tasarlamak için öncelikle oyunda yer alacak objelerinin pozisyonlarını hesaplamamız gerekiyor. Canvasta (0, 0) noktasının pencerenin sol üst köşesine geldiğini ve bir obje eklerken objenin sol üst köşesinin koordinatını hesaplamız gerektiğini de derste öğrenmiştik. Oyundaki objelerin (yol çizgileri, arabalar, skor yazısı) pozisyonlarını hesaplamak için aşağıda bulunan sunumdan faydalanabilirsiniz.

## Oyun Videosu
[Buraya tıklayarak](https://drive.google.com/file/d/1Z0V48Gl_6YYi195LPJJorN54yS1gZmwn/view?usp=sharing) oyunun videosuna ulaşabilirsiniz.

## Oyun Tasarımı
<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vS9DXKtrTWnZI4Z0yHsExtX7jlPuWO7IR7lhK5HWuGD4jmeFfBpx99hWGI81lM6Ezf6NYemvMyHusam/embed?start=false&loop=true&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/file/d/11sNyDoHvQZDq_7fFcLtzTuIjI40emj9a/view?usp=sharing) bu haftaya ait çalışmaların başlangıç kodlarına ve oyundaki araba resimlerine ulaşabilirsiniz.

# Ekstra Egzersizler

## Ekstra Egzersiz 1

Kasiyer Selin Hanım müşterilerin aldıkları ürünlerin fiyatlarının toplamını bulmak istiyor. Ona yardımcı olmak için bir program hazırlayalım. Selim Hanım girdi olarak 0 girene kadar ürünlerin fiyatları toplanmaya devam etmelidir.

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

## Egzersiz 2

Özellikle şu zamanlarda zamanı kontrol etmek çoğumuz için zor oluyor. Sevdiğimiz şeyler üzerinde daha çok zaman harcamayı tercih ederken sorumluluklarımızı da aksatmamaya çalışıyoruz. Bize bir şey üzerinde yeterince uğraştığımızı verdiğimiz süre içerisinde geriye doğru sayarak ve bittiğinde de bildiren bir program yazalım.

Not: Programın her bir saniyede çalışması için time kütüphanesini projeye dahil etmeyi ve time.sleep(saniye) fonksiyonunu kullanmayı unutma! Bu fonksiyon programın "saniye" kısmına girdiğiniz süre kadar beklemesini sağlar.

```
# Örnek Çalışma Şekli

> Seni süre bittiğinde uyarmam için kaç dakika geçmeli? 360
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

## Egzersiz 3

1 den büyük asal olmayan bir tamsayının rakamları toplamı, sayının çarpanlarına ayrılarak yazıldığında, bu yazılışta bulunan tüm asal sayıların rakamlarının toplamına eşitse bu sayı bir Smith sayısıdır. 
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
