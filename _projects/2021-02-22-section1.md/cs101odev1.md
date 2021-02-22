---
layout: post
title: Ödev 1
subtitle: Değişkenlere giriş, veri türleri, print ve input
categories: odev
authors: [Oya Suran, Rıdvan Balamur]
tags: [odev]
slug: odev1
---

Bu ödevin teslim tarihi *1 Mart Pazartesi 22.00*'dır. Ödevinizi bitirdiğinizde Ed üzerinden teslim etmeyi unutmayın. Bu konuda 
paylaştığımız [bu gönderi](https://edstem.org/us/courses/4754/discussion/267387) faydalı olacaktır.

Unutmayın, ödevler hem konuları pekiştirmenize yarar hem de programdan sertifika alabilmek için gereklidir.
 
## Başlangıç Kodları
<!-- todo update -->
[Buraya tıklayarak](https://drive.google.com/file/d/1WPlPJYXfvN-HfmaeL5KrHlFpM7zMrGgo/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

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

Pelin, Selin ve Perseverance Rover'ının maceraları devam ediyor. Mars'a başarılı bir şekilde ulaşan üçlü şimdi Mars'tan belirli bir taş alıp ağırlığını hesaplayıp, Dünya'ya götürmeli ve orada tekrar ağırlık ölçümleri yapmalılar. Son olarak tekrar Dünya'dan Mars'a dönmeliler. 

**Unutmayın biz zaten `yolculuk` fonksiyonunu Hafta 1 Grup Çalışmasında yazmıştık.**


![](https://www.haveeru.com.mv/wp-content/uploads/2020/11/NASA-is-advancing-to-bring-Mars-rocks-back-to-Earth-796x445.jpg)

İlk olarak `yolculuk` fonksiyonunu tekrar doldurmalısınız (Hafta 1 Egzersiz 2'den kopyalayabilirsiniz).
Bunun yanı sıra herhangi bir gezegen için ağırlık hesaplaması yapan bir fonksiyon yazmalısınız. Bunun için 
başlangıç kodunda verile `agirlik_hesaplama` fonksiyonunu kullanabilirsiniz. Bu fonksiyonu 
hem Mars'taki hem de Dünya'daki ağırlık için ortak kullanacaksınız. Bu fonksiyon önce kullanıcıya
bulunduğu gezegenin ivmesini sormalı ve sonra aşağıdaki formulü kullanarak ağırlık hesaplamayıp 
kullanıcıyı bilgilendirmelidir.

```ağırlık = kütle * gök cisminin çekim ivmesi ```

İstediğiniz çekim ivmesini girebilirsiniz. Taşın kütlesi ve uzaklık size `TAS` ve 
`UZAKLIK` sabitleri ile kodda verilmiştir.


```
# Örnek Çalışma Şekli

> Bulundugunuz gezegenin yercekim ivmesini giriniz: 10
> Taşın şu andaki ağırlığı  15.0
> Roketinizin hızı (km/saat): 454554
> Gidiş süreniz hesaplandı..
> Yolculuk süreniz yaklaşık 455 saattir.
> Bulundugunuz gezegenin yercekim ivmesini giriniz: 34
> Taşın şu andaki ağırlığı  51.0
> Roketinizin hızı (km/saat): 34343
> Gidiş süreniz hesaplandı..
> Yolculuk süreniz yaklaşık 6023 saattir.
> Görev tamamlandı. Bir sonraki görevde görüşmek üzere.

```
