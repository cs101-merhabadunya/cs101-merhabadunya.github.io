---
layout: post
title: Hafta 1 - Grup Çalışması Egzersizleri
subtitle: Değişkenlere giriş, veri türleri, print ve input
categories: grup çalışması
authors: [Oya Suran, Rıdvan Balamur]
tags: [grup çalışması]
# slug: hafta1-grup
permalink: /2021guz/projeler/hafta1-grup
---

## Başlangıç Kodları
[Buraya tıklayarak](https://drive.google.com/file/d/1uNTIOTexY_SmmVNwKUN2eC7axsRSNdRY/view?usp=sharing) problemlere ait başlangıç kodlarına ulaşabilirsiniz.

## Grup Çalışması - Hafta 1

### Egzersiz 1

Bir yapay zeka şirketi yeni çıkaracakları robotun insanları selamlamasını istemektedir. Robot kullanıcıdan ismini girdi olarak alıp kullanıcıyı ismiyle selamlamaktadır. Ayrıca onlara doğdukları yılı sorup aralarındaki yaş farkını söyleyecektir. Robot yeni geliştirildiği için doğum yılı 2021. Bu işlevleri sağlayan, kullanıcıdan ismini girdi olarak alıp onu selamlayan, ve doğum yılını alıp bunu bir değişkene kaydedip gerekli işlemleri yapacak bir program parçası yazınız.

![](https://specials-images.forbesimg.com/imageserve/5f8247cf2190cd26e6fe7b90/960x0.jpg?fit=scale)

```
# Örnek Çalışma Şekli

> Adınız?: Rıdvan
> Merhaba, Rıdvan!
> Rıdvan, hangi yıl doğdun?: 2006
> Aramızdaki yaş farkı 15 yıl.

```

### Egzersiz 2

Bir maceraya atılmaya karar vermiş iki kardeş, Selin ve Pelin. Dünyadan Mars'a Perseverance Rover'ıyla Mars'tan bazı taşlar alıp analiz etmeye çalışacaklardır. Bu macera için de sizin yardımınıza ihtiyaçları var. 

**NOT: Bu görev iki parçadan oluşmakta ilk parçasını egzersiz 2'de ikinci parçasıysa Ödev 1 - Egzersiz 2'de yapacağız.**

![](https://cdn.vox-cdn.com/thumbor/gtFX_9BVO5yj51Pr5vDq9JOYrlY=/0x0:3000x1688/1200x800/filters:focal(1213x757:1693x1237)/cdn.vox-cdn.com/uploads/chorus_image/image/68831020/09_Touchdown_10k.0.jpg)

 Görevin bu kısmında kardeşler Mars'a gitmeli. Kardeşleri Mars'a yollamak için size verilen `yolculuk` fonksiyonunu tamamlamalısnız.
 Bu fonksiyon:
 1. Kullanıcıdan roketin hızını almalı. Hız km/saat cinsinden.
 2. Roketin Mars'a ne kadar sürede ulaşacağını (saat cinsindem) hesaplamalı ve kullanıcıya süreyi bildirmeli (yani konsola yazdırmalı). Süreyi hesaplamak için kullanacağınız formül aşağıda verilmiştir: 
> Dünya-Mars arası uzaklık başlangıç kodunda `UZAKLIK` isimli sabitle verilmiştir.

```
Zaman = Yol/Hız
```

Programı yazmayı bitirdiğinizde aşağıdaki gibi bir çalışma şekli gözlemlemelisiniz.

```
# Örnek Çalışma Şekli

> Roketinizin hızı (km/saat): 5656666
> Gidiş süreniz hesaplandı..
> Yolculuk süreniz yaklaşık 36 saattir.
> Görev tamamlandı. Bir sonraki görevde görüşmek üzere.
```
