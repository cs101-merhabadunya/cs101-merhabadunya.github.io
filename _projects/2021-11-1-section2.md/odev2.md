---
layout: post
title: Ödev 2
subtitle: Değişken türleri, Basit Operatörler, Kontrol yapıları
categories: ödev
authors: [Eren Çetin, Barkın Kara]
tags: [odev]
slug: odev2
---

Bu ödevin teslim tarihi *8 Kasım Pazartesi 22.00*'dır. Ödevinizi bitirdiğinizde Ed üzerinden teslim etmeyi unutmayın.

Unutmayın, ödevler hem konuları pekiştirmenize yarar hem de programdan sertifika alabilmek için gereklidir.

## Başlangıç Kodları
<!-- todo update -->
[Buraya tıklayarak](https://drive.google.com/file/d/1W24Sy3fvXm0uZnCG47wOkVjv0YnRHX3r/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1

Bozuk bir hesap makinesi ondalıklı sayılarla işlem yaparken yanlış sonuç vermektedir.
İşleme dahil olan her ondalıklı sayıyı yuvarlayarak işlemi yapan hesap makinesinin
kullanıcı tarafından verilen işlemin sonucunu kaç bulacağını hesaplayan bir program
yazalım. Programda kullanıcıdan 3 tane input almalısınız. Bunların
- Birincisi işlem yapılan ilk sayı.
- İkincisi işlem yapılan ikinci sayı.
- Üçüncüsüyse işlem tipi. İşlem tipi çarpma, toplama ve çıkarmadan biri olabilir. Kullanıcı eğer çarpma işlemi yapmak istiyorsa input olarak *, çıkarma işlemi yapmak istiyorsa -, toplama yapmak istiyorsa + verecektir.

![](https://image.freepik.com/free-vector/illustration-calculator-machine_53876-5566.jpg)

Yuvarlarken 0.5 ve üzerini bir üst tam sayıya, 0.5'ten küçük ondalıkları bir alt tam sayıya
yuvarlayabilirsiniz.

```
# Örnek Çalışma Şekli
> Sayı 1: 2.75
> Sayı 2: 3.33
> İşlem: +
> Sonuç: 6
# Yuvarlayarak işlem yaptığı için 2.75'i 3, 3.33'ü 3 olarak işleme aldı. Dolayısıyla sonucu 3+3'ten 6 buldu.
```

## Egzersiz 2

Tatil için Amerika'ya gidecek olan Barkın'ın uçağa binişte valizini teslim etmesi gerekiyor. Ancak yanına çok fazla kıyafet 
aldığı için ekstra ücret ödemesi gerekebilir. Bu durumda Barkın gibi yolcuların ne kadar fazla ücret ödemesi gerektiğini 
anlamak için havaalanı şirketinin bir Python koduna ihtiyacı var. Yardımcı olabilir misiniz?

![](https://i4.hurimg.com/i/hurriyet/75/0x0/5a7d4d6fc03c0e239419e3dd.jpg)

Valizin kütlesini kullanıcıdan input olarak aldıktan sonra ücreti hesaplayalım. 
Havaalanı şirketi valizin kütlesi tam sayı olmadığında her zaman yüksek olan tam sayıya yuvarlamayarak ekstra 
ücreti hesaplamayı tercih ediyor. Kodu tamamladığınızda aşağıdaki gibi bir çalışma şekli göreceksiniz.

```
# Örnek Çalışma Şekli 1

> Valizinizin kütlesini giriniz: 16.240
> Valiz tarifemiz:
> (0-15 kg) = 65 TL (Sabit fiyat)
> (15-20 kg) = 10 TL/kg
> (>20 kg) = 20 TL/kg
> Ödemeniz gereken ekstra ücret 20 TL.
> Ödemeniz gereken total ücret 85 TL.

# Örnek Çalışma Şekli 2

> Valizinizin kütlesini giriniz: 22.360
> Valiz tarifemiz:
> (0-15 kg) = 65 TL (Sabit fiyat)
> (15-20 kg) = 10 TL/kg
> (>20 kg) = 20 TL/kg
> Ödemeniz gereken ekstra ücret 110 TL.
> Ödemeniz gereken total ücret 175 TL.
```

## Egzersiz 3

Amerika'ya varan Barkın haberlerde hava sıcaklığını hep Fahrenheit cinsinden gördüğü için sorun yaşıyor. 
Barkın'a yardımcı olmak için hava sıcaklığını Fahrenheit'tan Celcius'a veya Celcius'tan Fahrenheit'a çevirecek bir program hazırlayalım.

![](https://s3.r29static.com/bin/entry/b34/0,0,2000,1050/x,80/2097921/image.jpg)

İlk olarak `fahrenheit_celcius` ve `celcius_fahrenheit` fonksiyonlarını dolduralım.

Barkın'a öncelikle hava sıcaklığını ve hangi türde hava sıcaklığı vereceğini sorup, aldığımız yanıta göre 
doğru fonksiyonu kullanarak çevirme işlemini tamamlayalım. Son olarak yeni türdeki hava sıcaklığını yazdıralım. 
Eğer Fahrenheit (F) veya Celcius (C) cinsinden hava sıcaklığı almazsak kullanıcıyı uyaralım!

Barkın hava sıcaklığındaki ondalık değişimleri umursamadığı için sonucu en yakın ondalık sayıya yuvarlayalım!

```
(°F - 32) * (5 / 9) = °C
```

Çevirme işlemi için doğru fonksiyonları hazırlamak için yukarıdaki formülü kullanabilirsiniz.

```
# Örnek Çalışma Şekli

> Hava sıcaklığı: 77
> Sıcaklık birimi (F veya C): F
> Celcius cinsinden hava sıcaklığı: 25
```