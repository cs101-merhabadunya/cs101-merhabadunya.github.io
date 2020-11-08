---
layout: post
title: Hafta 2 - Grup Çalışması Egzersizleri
subtitle: Temel Operatörler, Dallanma, Temel Düzeyde Fonksiyonlar ve For Döngülerine Giriş 
authors: [Necla Mutlu, Ahmet Uyar, İdil Defne Çekin]
categories: grup çalışması
tags: [grup çalışması]
slug: hafta2-grup  # link is generated as /projeler/hafta2
---
## Başlangıç Kodları
[Buraya tıklayarak](https://drive.google.com/file/d/1YGeGMTZT6yuBbOobX6FsxilN1M3i3xA6/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1

Bazı ebeveynler çocuklarının saat kaça kadar televizyon izleyebileceklerini kontrol etmek ister. Bu egzersizde yazacağınız programda kullanıcının yaşını girdi olarak almalısınız. Eğer kullanıcının yaşı 12'yse veya 12'den küçükse, saatin kaç olduğunu kontrol etmelisiniz. Saat 19.00'dan erkense 12 yaşından büyük olmayan kullanıcılara televiyon izlemelerine izinleri olduğunu, değilse izinleri olmadığını ekrana yazdırmalısınız. 12 yaşından büyükler için bir sınırlama bulunmamaktadır.
Size verilen başlangıç kodunda **televizyon_izleyebilir_mi()** fonksiyonu bulunmaktadır. Bu fonksiyon kullanıcı 12 yaşından küçükse televizyon izlemeye izni olup olmadığını öğrenmek için kullanılmalıdır. Fonsksiyonun içerisinde şu an bulunduğumuz zamanı Saat:Dakika:Saniye formatında "**zaman**" adlı değişkene sizin için atadık. "**zaman**" değişkeni **string** tipinde bir değişkendir. Bu bilgiler ışığında **televizyon_izleyebilir_mi()** fonksiyonunu ve programınızın akışını sağlayacak ana fonksiyonu tamamlayınız.

![](https://burst.shopifycdn.com/photos/man-holding-clock-forward.jpg?width=700&format=pjpg&exif=0&iptc=0)

## Egzersiz 2

İki mühendis önemli bir mesajın gizlice iletilmesini sağlamak için RSA şifreleme algoritması üzerinde çalışıyorlar. Bu şifreleme sisteminde mesajın şifrelenebilmesi için 2 adet asal sayıya ihtiyaç duyuluyor. Bu yüzden mühendisler akıllarına gelen bir sayının asal olup olmadığını belirleyecek bir programa ihtiyaç duyuyorlar. Girdi olarak verilen bir sayının asal olup olmadığını ekrana yazdıran bir program hazırlayınız. 

![](https://images.pexels.com/photos/1314543/pexels-photo-1314543.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940)

## Egzersiz 3

Cız bız, çocukların bölmeyi öğrenmesi için oynanan bir oyundur. Oyuncular sırayla belli bir sayıya kadar sayarlar ancak dikkat etmeleri gereken kurallar vardır:
- Üçe bölünebilen bir sayı "Cız" kelimesiyle, 
- Beşe bölünebilen bir sayı "Bız" kelimesiyle,
- On beşe bölünebilen bir sayı "CızBız" ile ifade edilmelidir.
- Diğer sayılar olduğu gibi söylenir.
Size verilen başlangıç kodunu kullanarak kullanıcıdan kaça kadar saymak istediğini alıp başarılı bir Cız Bız oyununu konsola yazdırmanızı istiyoruz. Örnek vermek gerekirse:
```
# Örnek Çalışma Şekli

 Bir sayı giriniz: 5
 Bız

# Örnek Çalışma Şekli

 Bir sayı giriniz: 3
 Cız

# Örnek Çalışma Şekli

 Bir sayı giriniz: 15
 CızBız

# Örnek Çalışma Şekli

 Bir sayı giriniz: 4
 4
```

## Ekstra Egzersizler

## Egzersiz 1 

Bu programda **for** döngüsünün nasıl çalıştığına dair bir örneğimiz bulunmakta. Kullanıcıdan 1 ile 10 arasında bir sayı istenecek ve bu sayı adedince kendinizi tanıtmanız istenecektir.
Size verilen başlangıç kodunda **kendini_tanıt()** fonksiyonu bulunmaktadır. Bu fonksiyonu, konsola kendi isminizi yazdıracak şekilde düzenlemeniz istenecektir. 

```
# Örnek Çalışma Şekli

Bir sayı giriniz: 3
Benim adım Idil
Benim adım Idil
Benim adım Idil
----------------
# Örnek Çalışma Şekli

Bir sayı giriniz: 12
Error
```


## Egzersiz 2 

Artık yıl, Miladi takvimde 365 yerine 366 günü olan yıldır. Dört yılda bir yapılan bu uygulamanın nedeni Dünya'nın Güneş çevresinde dönme süresinin (astronomik yıl), Güneş'in aynı meridyenden iki kez geçişi arasındaki ortalama zamanın (gün) tam katı olmamasıdır. Bir astronomik yıl yaklaşık olarak 365,242 gün olmasına rağmen normal bir takvim yılı 365 gündür.
Bir yılın artık yıl olarak adlandırılabilmesi için bu yılın dört ile bölünebilmesi gerekir. Fakat bu yıl yüz ile bölünebiliyorsa aynı zamanda dört yüz ile bölünebilmelidir. Geriye kalan yıllar artık yıl sayılmazlar. 
Size verilen başlangıç kodunda kullanıcıdan bir yıl istemenizi, ardından da bu yılın artık yıl olup olmadığını kullanıcıya bildirmeniz istenecektir. 

```
# Örnek Çalışma Şekli

 Yılı giriniz: 2004
 Artık yıl

# Örnek Çalışma Şekli

 Yılı giriniz: 1900
 Artık yıl değil

# Örnek Çalışma Şekli

 Yılı giriniz: 48
 Artık yıl

# Örnek Çalışma Şekli

 Yılı giriniz: 2003
 Artık yıl değil

```
