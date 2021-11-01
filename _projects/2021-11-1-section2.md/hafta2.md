---
layout: post
title: Hafta 2 - Grup Çalışması Egzersizleri
subtitle: Değişken türleri, Basit Operatörler, Kontrol yapıları
categories: grup çalışması
authors: [Barkın Kara, Eren Çetin]
tags: [grup çalışması]
slug: hafta2-grup
---

## Başlangıç Kodları
<!-- todo update -->
[Buraya tıklayarak](https://drive.google.com/file/d/1b0yBbDFgFt7Fe80-VXR91uyKAOUfKyxS/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1

Matematik öğretmenliği yapan Selin, öğrencilerinin ortalamalarına göre harf notlarını belirleyen bir fonksiyon
yazmak istemektedir.Aynı zamanda öğrencilerine not ortalamaları konusunda yardımcı olmak isteyen Selin öğretmen,
bütün öğrencilerine ortalamalarını bir yüksek tam sayıya yuvarlama sözü vermiştir.

Selin öğretmenin belirlediği not aralıkları

- 100-88 arası A
- 88-75 arası B
- 75-62 arası C
- 62-49 arası D
- 49 ve altı F
şeklinde olduğuna göre;

İlk olarak öğrencilerden girdikleri iki sınavdan ve proje ödevlerinden aldıkları notları girdi olarak alıp bunların ortalamasını
hesaplayan, ardından da bu ortalamayı bir yüksek tam sayıya yuvarlayıp buna  göre öğrencilere bir harf notu atayan bir fonksiyon
yazmasında Selin öğretmene yardım edelim. F alan öğrencilere daha çok çalışmaları yönünde bir uyarı vermeyi de unutmayın.

![](https://us.123rf.com/450wm/chereliss/chereliss1710/chereliss171000011/87525257-fail-grade-result-f-hand-drawn-vector-grade-with-minus-in-circle-flat-illustration.jpg?ver=6)

```
# Örnek Çalışma Şekli

>Birinci sınav notun nedir?:61
>İkinci sınav notun nedir?:54
>Proje ödevi notun nedir?:83
>Ortalaman 67 harf notun ise C 
```

## Egzersiz 2

CızBız, çocukların bölmeyi öğrenmesi için oynanan bir oyundur. Çocukların bölünebilme kurallarını daha iyi öğrenebilmesi için
üçe bölünebilen bir sayı için "Cız" ,beşe bölünebilen bir sayı için  "Bız" ,  on beş ile bölünebilen  bir sayı için ise konsola 
"CızBız" yazdıran bir program hazırlamanızı istiyoruz.  .Eğer sayı üç,beş veya on beşten herhangi birine bölünmüyor ise direk 
sayının kendisi konsola yazdırılacak ve bu sayı kullanıcıdan istenilecektir.Farklı sayıları denemek için kod tekrar tekrar 
çalıştırılabilir.

![](https://www.pngkey.com/png/detail/895-8951628_student-learning-writing-boy-doing-homework-drawing.png)

```
# Örnek Çalışma Şekli
>Lütfen bir sayı giriniz:9
>Cız

>Lütfen bir sayı giriniz:25
>Bız

>Lütfen bir sayı giriniz:45
>CızBız

>Lütfen bir sayı giriniz:23
>23
```

## Egzersiz 3

Üniversiteyi yeni bitiren yakın arkadaşınız Murat mühendis olarak  bir şirkette ilk işine başlamıştır. Esnek çalışma saatleri ile
çalışmayı kabul ettiği için haftalık standart bir çalışma süresi olmayan Murat, bu sebeble maaşını hesaplama konusunda sorun
yaşamış ve sizden yardım istiyor. İş sözleşmesini sizinle aşağıdaki gibi paylaşan Murat'a , girdiği çalışma saatine göre maaşını
hesaplayan ve eğer mesai yapmışsa da toplam kaç saatlik mesai yaptığını  geri dönen bir fonksiyon yazarak  yardım etmelisin.

İş Sözleşmesi

- Saatlik ücret 42 TL
- Haftalık normal çalışma saati = 45
- 45 saat üzeri her çalışma saati fazla mesai kabul edilir
- Fazla mesailerin saatlik ücreti normal ücretin 1.5 katıdır

![](https://www.optimaldenetim.com/wp-content/uploads/2018/09/para-sayan-insan.jpg)

```
# Örnek Çalışma Şekli

>Haftalık toplam çalışma saatin ne?:40
>Bu hafta fazla mesai yapmamışsın maaşın =1680.0TL

              veya mesai yapmışsa

>Haftalık toplam çalışma saatin ne?:53
>Bu hafta toplam 8.0 saat fazla mesai yapmışsın.
>Maaşın =2394.0 TL
```
