---
layout: post
title: Hafta 5 - Grup Çalışması Egzersizleri
subtitle: Grafik, While loop
categories: grup çalışması
authors: [Yağmur Akarken, Cemal Efe Gayir]
tags: [grup çalışması]
slug: hafta5-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/file/d/13jqb97B3xmuPJ8M8Umm8rVcvToLDzgRZ/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Grup Çalışması - Hafta 5

### Egzersiz 1

**Fiş oluşturmaya yardım edelim!**

![](https://www.blog.modernraf.com.tr/wp-content/uploads/2020/11/market-raf-duzeni-nasil-olmali.jpeg-1-780x400-1.jpg)

 Bir markette barkod okuyucu sistem bozulmuştur. Bu yüzden kasiyerler her ürün için fiyatlara bakıp
    hesap makinesiyle fiş tutarını hesaplamaktadırlar. Biz de onlara yardımcı olmak için fiş yazdıran
    ve toplam tutar hesaplayan bir program yazacağız.

 Marketle ilgili bilmemiz gerekenler şunlar:
 Markette iki çeşit ürün var: Biri kg olarak satılan ürünler diğeri de paket olarak satılan ürünler.
 İşimizi kolaylaştırmak için market çalışanları bu ürünleri ve ürünleri fiyatlarını listelediler.

  kg_urun_listesi=["elma","portakal","muz", "domates","kabak","marul"]
  kg_urun_fiyat_listesi=[2.25, 4.50, 10.0, 8.75, 8.50, 10.10]

  Buradan da anlaşılacağı gibi; elmanın 1 kg'lık için fiyatı 2.25, portakalın 1 kg'lık fiyatı 4.50...

  Gelen her müşteri için hangi ürünü aldıkları, aldıkları kg cinsinden satılan bir ürün ise kaç kg aldığı,
  paket cinsindense kaç paket aldığını soracağız ve bir ürün için ödemesi gereken fiyati, ürünün adını listelere
  kaydedeceğiz.
  Eğer ürün adı olarak bitti girilirse program yeni ürünler sormaya devam etmeyecek.

  Sonrasında bu listeler üzerinde gezinip fişi bastıracağız.


```
-------------Örnek çalışma şekli-------------
Merhabalar, toplam fiyatı öğrenmek için ürünleri ve fiyatları girmeye başlayabilirsiniz!
    > Ürün adını giriniz: konserve
    > Kaç paket konserve aldınız?: 3
    > Ürün adını giriniz: portakal
    > Kaç kg portakal aldınız?: 1.5
    > Ürün adını giriniz: marul
    > Kaç kg marul aldınız?: 0.5
    > Ürün adını giriniz: çikolata
    > Kaç paket çikolata aldınız?: 3
    > Ürün adını giriniz: bitti

    > konserve  -> 60.0
    > portakal  -> 6.75
    > marul  -> 5.05
    > çikolata  -> 21.75
    > Toplam fiyat: 93.55
    
-----------Örnek çalışma şekli sonu-----------

```

### Egzersiz 2

![](https://im.haberturk.com/2021/02/28/ver1614497754/2988400_810x458.jpg)

Hava durumu üzerine çalışan bilim insanları sizden yapmak istedikleri yağmur simülasyonu için yardım istemiştir. Ancak bu simülasyonu yazarken sizden farklı türde yağmurları farklı renklerle ifade etmenizi istemişlerdir. Kodunuzu yazmadan önce de size bir liste içinde yağmur damlalarının sayısını vermişlerdir.

YAGMUR_SAYILARI  = [100, 200, 150, 300]

Bu bilim insanları sizden sırayla verilen sayıda yağmur damlasını yağdırma animasyonunu yapıp, listede verilen bir sonraki damla sayısına geçmenizi istemişlerdir. Her bir yağmur damlası türü için renkler rasgele seçilecek fakat hiçbir zaman tekrar aynı renk kullanılmayacaktır.

Örnek çalışma için dosyaların içinde gönderdiğimiz .gif dosyasına bakabilirsiniz.

