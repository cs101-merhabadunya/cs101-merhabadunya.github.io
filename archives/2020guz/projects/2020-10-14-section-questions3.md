---
layout: post
title: Hafta 3 - Grup Çalışması Egzersizleri
subtitle: For Döngüleri ve Fonksiyonlar
categories: grup çalışması
authors: [Ahmet Uysal, Oya Suran]
tags: [grup çalışması]
permalink: /2020guz/hafta3-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/file/d/12NJZV1FUK3DB2T8ZT90Ew6Ti_z_K3sKs/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1

Arkadaşlarını için yemek siparişi verecek olan Cenk 5 farklı çorbadan 2 tanesini, 12 ana yemekten 4 tanesini ve 3 tatlıdan 1 tanesini seçmesi gerekmetedir. Cenk'in bu seçimi kaç farklı şekilde yapabileceğini bulmak için size verilen başlangıç kodundaki `kombinasyon` ve `faktöriyel` fonksiyonlarını tamamlayınız.

**Cevap**: 14850

![Yemek Masası](https://images.pexels.com/photos/54455/cook-food-kitchen-eat-54455.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940)

## Egzersiz 2

Bu egzersizde 3 farklı fonksiyon hazırlayıp, kullanıcıdan bu fonksiyonlardan birini seçmesini ve
o fonksiyona göre girdileri isteyip, bu fonksiyonun sonucunu konsola bastırıyoruz.

```
# Örnek Çalışma biçimi:

# 1. Fonksiyon için
> Hangi fonksiyonu kullanmak istiyorsun? 1
> Bu fonksiyonu kullanmak için kelime giriniz: kelime
> Bu fonksiyonu kullanmak için sayı giriniz: 2
Sonucunuz 3

# 2. Fonksiyon için
> Hangi fonksiyonu kullanmak istiyorsun ? 3
> Bu fonksiyonu kullanmak için sayı giriniz: 10
Sonucunuz 25

# 3. Fonksiyon için
> Hangi fonksiyonu kullanmak istiyorsun? 3
> Bu fonksiyonu kullanmak için sayı giriniz: 7
Sonucunuz 14
```

## Egzersiz 3

Bu egzersizde konsola bir çam ağacı çizeceğiz.

Kullanıcıdan çam ağacının uzunluğu almalı ve bu ağacı konsola yazdırmalısın.

```
# Örnek Çalışma Şekli

> Lütfen istediğiniz ağacın uzunluğunu girin: 5
    *
   * *
  *   *
 *     *
*       *
   | |

# Örnek Çalışma Şekli 2

> Lütfen istediğiniz ağacın uzunluğunu girin: 8
       *
      * *
     *   *
    *     *
   *       *
  *         *
 *           *
*             *
      | |
```

![Yılbaşı Ağacı](https://images.pexels.com/photos/936706/pexels-photo-936706.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260)

# Ekstra Egzersizler

## Ekstra Egzersiz 1

Çocukken insanların dediklerini taklit edip kendi aramızda eğlenirdik.
Fakat maalesef büyüyünce bunun yanlış bir şey olduğunu öğrenip bundan vazgeçtik.
Neyse ki bu terbiyesizliği bizim yerimize yapması için bir program yazabiliriz!

Kullanıcıdan bir yazı girmesini isteyip bu yazıdaki tüm sesli harfleri o
ile değiştirip konsola basan bir program yaz.

**İpucu**: `str` türünde bir değerin başka bir stringing içinde olup olmadığını `in` operatörünü kullanarak öğrenebilirsin. Örneğin `'a' in 'ahmet'` ifadesi `True` değerini, `'a' in 'Ahmet'` ifadesi `False` değerini verir.

```
# Örnek Çalışma Şekli

> Bana kendini anlat: Ben Ahmet, bisiklete binmeyi çok severim.
Bon Ohmot, bosokloto bonmoyo çok sovorom.
```

![](https://images.pexels.com/photos/3812738/pexels-photo-3812738.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940)

## Egzersiz 2

Cız bız, çocukların bölmeyi öğrenmesi için oynanan bir oyundur. Oyuncular sırayla belli bir sayıya kadar sayarlar ancak dikkat etmeleri gereken kurallar vardır:

- Üçe bölünebilen bir sayı "Cız" kelimesiyle,
- Beşe bölünebilen bir sayı "Bız" kelimesiyle,
- On beşe bölünebilen bir sayı "CızBız" ile ifade edilmelidir.
- Diğer sayılar olduğu gibi söylenir.

Size verilen başlangıç kodunu kullanarak kullanıcıdan kaça kadar saymak istediğini alıp başarılı bir Cız Bız oyununu konsola yazdırmanızı istiyoruz. Örnek vermek gerekirse:

```
# Örnek Çalışma Şekli

> Bir sayı giriniz: 23
1
2
Cız
4
Bız
Cız
7
8
Cız
Bız
11
Cız
13
14
CızBız
16
17
Cız
19
Bız
Cız
22
23
```
