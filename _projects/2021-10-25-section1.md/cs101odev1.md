---
layout: post
title: Ödev 1
subtitle: Değişkenlere giriş, veri türleri, print ve input
categories: odev
authors: [Oya Suran]
tags: [odev]
slug: odev1

---

Bu ödevin teslim tarihi *1 Kasım Pazartesi 22.00*'dır. Ödevinizi bitirdiğinizde Ed üzerinden teslim etmeyi unutmayın.

Unutmayın, ödevler hem konuları pekiştirmenize yarar hem de programdan sertifika alabilmek için gereklidir.
 
## Başlangıç Kodları
<!-- todo update -->
[Buraya tıklayarak](https://drive.google.com/file/d/1Yxq1P1kK8RGchMMHp3OFKorlCflxxAz0/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Egzersiz 1

Program boyunca çözeceğimiz birçok egzersizin aksine bu sefer tüm kodu biz size veriyoruz. 
Ama ne yazık ki kodu yazan arkadaşlarımızdan biri sınavlara 
çalışmaktan bitap düşüp kodda bazı hatalar yapmış bu sebepten kodu çalışmıyor. 
Bu arkadaşımızın yorulup umutsuzluğa kapılmasını engelleyip kodunu doğru çalıştırmasına 
yardım etmeliyiz.

![](https://www.meme-arsenal.com/memes/5ddb6d31fed63b9f72f9544842b8cbbb.jpg)

Kodu düzelttiğinizde aşağıdaki gibi bir çalışma şekli göreceksiniz.

```
# Örnek Çalışma Şekli

> Yanlış çalışıyorum niye ki
> Bazı boşluk düzenlerine dikkat etmediğim için olabilir mi?
> Lütfen bir sayı giriniz:6
> Girdiğin sayının 5 fazlası  11 dır.
> Beni çağırmazsan ben gelmem ki
> Aynı zamanda hep boşluklara dikkat etmen lazım
> İşte şimdi başardın

```

## Egzersiz 2

Acaba çok mu dizi izliyorum sorusunu kendine sormaya başlayan Efe için bir program hazırlamalısınız.

![](https://i.pinimg.com/736x/f8/41/ce/f841ce59a11caffd7d0f0ceb3b030e4a.jpg)

Bu programda kullanıcıdan aşağıdaki dört bilgiyi almalısınız:
1. Dizinin ismi
2. Sezon sayısı
3. Sezondaki bölüm sayısı
4. Bir bölümün oralama süresi

Aldığımız bu bilgilerin sonucunda kullanıcının bu dizi için toplamda ne kadar süre harcadığını hesaplayıp konsola yazdırarak kullanıcıyı bilgilendirmelisiniz.
Programı yazmayı bitirdiğinizde aşağıdaki gibi bir çalışma şekli gözlemlemelisiniz.

```
# Örnek Çalışma şekli:

> En son izlediğiniz dizinin ismini giriniz:Leyla ile Mecnun
> Kaç sezon izlendi:10
> Bir sezon kaç bölüm:15
> Bir bölümün (ortalam) süresi (dk):60
> Leyla ile Mecnun dizisi toplam  150 saat izlendi.

```

## Egzersiz 3

Pelin, Selin ve Jeff Bezos'un maceralari devam ediyor.
Plüton'a başarılı bir şekilde ulaşan üçlü şimdi Plüton'da klişe yapılması gereken ağırlık ölçümü yapacaklardır, Pelin ve Selin'in kütlelerini biz size verdik ama Jeff'in kütlesini kullanacıya sorup
ağırlık hesaplamanız lazım,
Sonra Dünya'ya dönmeli ve orada tekrar ağırlık ölçümleri yapmalısınız. 

**Unutmayın biz zaten `yolculuk` fonksiyonunu Hafta 1 Grup Çalışmasında yazmıştık.**


![](https://www.kreatifbiri.com/wp-content/uploads/2018/09/992B0F2D-3C2D-469F-B828-D14EB1A28D26.jpeg)

İlk olarak `yolculuk` fonksiyonunu tekrar doldurmalısınız (Hafta 1 Egzersiz 2'den kopyalayabilirsiniz).
Bunun yanı sıra herhangi bir gezegen için ağırlık hesaplaması yapan bir fonksiyon yazmalısınız. Bunun için 
başlangıç kodunda verile `agirlik_hesaplama` fonksiyonunu kullanabilirsiniz. Bu fonksiyonu 
hem Plüton'daki hem de Dünya'daki ağırlık için ortak kullanacaksınız. Bu fonksiyon iki parametre alıyor (yerçekim ivmesi ve kütle) ve aşağıdaki formulü kullanarak ağırlık hesaplamayıp 
kullanıcıyı bilgilendirmelidir.

```ağırlık = kütle * gök cisminin çekim ivmesi ```

İstediğiniz çekim ivmesini girebilirsiniz. Pelin'in kütlesi  `P_KG`, Selin'in kütlesi `S_KG` ve uzaklık size
`UZAKLIK` sabitleri ile kodda verilmiştir.


```
# Örnek Çalışma Şekli

> Roketinizin hızı (km/saat): 45455446888
> Plütondaki yercekim ivmesini giriniz: 0.62
> Jeff Amca kaç kg?:  75
> Şu andaki ağırlığı: 46.5
> Şu andaki ağırlığı: 33.852
> Şu andaki ağırlığı: 30.07
> Gidiş süreniz hesaplandı..
> Yolculuk süreniz yaklaşık 11315 saattir.
> Dünyadaki yercekim ivmesini giriniz: 10
> Şu andaki ağırlığı: 750
> Şu andaki ağırlığı: 546
> Şu andaki ağırlığı: 485
> Görev tamamlandı. Bir sonraki görevde görüşmek üzere.

```
