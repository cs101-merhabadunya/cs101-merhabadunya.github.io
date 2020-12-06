---
layout: post
title: Hafta 6 - Grup Çalışması Egzersizleri
subtitle: str, set ve dict Veri Türleri
categories: grup çalışması
authors: [İdil Defne Çekin, Hasan Can Aslan]
tags: [grup çalışması]
slug: hafta6-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/file/d/1L9vezDDm1jqMqorIuAj-88XpNEq1xV_m/view?usp=sharing) bu haftaya ait çalışmaların başlangıç kodlarına ulaşabilirsiniz.


## Egzersiz 1 - Manav
Sanal bir manavın sipariş işlerini düenlemek için bir program yazalım. Depodaki ürünlerimizin adı ve miktarları depo isimli dictionary veri tipinde tutulmaktadır. Depodaki herhangi bir ürün bittiği zaman günlük satış hedefimize ulaşıyoruz ve manavı kapatıyoruz. Depodaki bütün ürünler doluyken, ürünlerden biri bitene kadar kullanıcıdan sipariş almamız gerekiyor.
Depodaki ürünlerin dolu olup olmadığını kontrol etmek için depo_dolu_mu(dict) fonksiyonunu dolduralım ve kullanalım.
Sipariş almak için öncelikle kullanıcıdan almak istediği ürünün adını alalım, sonra eğer ürün depomuzda varsa kullanıcıdan almak istediği miktarı öğrenelim. Eğer ürün yoksa, müşteriye o üründen satmadığımızı belirtelim. Eğer depomuzda o üründen istenilen miktarda bulunuyorsa o kadar ürünün teslimatını yapalım ve
depodaki ürün sayısını güncelleyelim. Eğer istenilen miktardan daha az ürün kaldıysa müşteriyi bu konuda bilgilendirelim ve elimizde olan miktarda ürün satalım.
Her satışın sonunda depodaki ürünlerimizi ve sayılarını konsolda gösterelim, bunun için depodaki_urunleri_goster(dict) fonksiyonunu kullanabiliriz.

```bash
#Örnek Çalışma Şekli 1

> Hangi ürünü almak istersiniz? Elma
> Kaç tane istersiniz? 25
> Elimizde 25 tane Elma kalmamış, size 20 tane veriyorum.
Elimizdeki ürünler:
0 tane Elma var
30 tane Portakal var
20 tane Muz var
25 tane Armut var
Bugünlük bu kadar satış yeter, dükkanı kapatalım.

#Örnek Çalışma Şekli 2:

> Hangi ürünü almak istersiniz? Kereviz
Bizim manavda Kereviz satılmıyor.
Elimizdeki ürünler:
20 tane Elma var
30 tane Portakal var
20 tane Muz var
25 tane Armut var
> Hangi ürünü almak istersiniz? Armut
> Kaç tane istersiniz? 25
Elimizdeki ürünler:
20 tane Elma var
30 tane Portakal var
20 tane Muz var
0 tane Armut var
Bugünlük bu kadar satış yeter, dükkanı kapatalım.
```

## Egzersiz 2 - Bozuk Yazıcı
Fırat Python dersini tekrar etmek için ders sunumlarını yazdırmaya karar verir. Hasan bunun doğaya ne kadar zararlı olacağını bilgisayarından da çalışabileceğini anlatsa da Fırat onu dinlemez ve kırtasiyeye gider. Tesadüf bu ya, ders sunumlarını bastırırken kırtasiyedeki yazıcı aniden bozulur ve bazı sayfaları tekrar çıkarır bazılarının da sırasını karıştırır. Tekrar çıkarmayı dener fakat makine yine aynı şekilde hatalı bastırır. Hadi Fırat'a sayfalarını düzenlemek için yardım edecek bir program yazalım. Önce sayfaları düzenleyeceğiz, daha sonra Fırat gibi doğaya zarar vermemek için tekrar eden sayfaları ayırıp, geri dönüşüm kutusuna atacağız.

Yapmamız gerekenler şöyle:
- Elimizde iki baskının sonucunda çıkan kağıtların sayfa numaralarından oluşan iki liste var.
- Bu iki listeyi birleştirip, sayfa numaralarına göre düzenlemeliyiz.
- Daha sonra tekrar eden sayfa numaralrını geri dönüşüm için ayırmalıyız.
- Son olarak Fırat'a vereceğimiz ve geri dönüşüm kutusundaki sayfaların numaralarını yazdıracağız

```bash
# Örnek Çalışma Şekli 
Merhaba Fırat. Lütfen doğayı korumak için kağıt israf etme.
Listeni düzenledim, işte sayfalar: [1, 2, 4, 5, 8, 9, 10, 12]
Geri dönüşüm kutusu: [1, 1, 1, 2, 2, 5, 8, 8, 8, 8, 10, 12, 12]
```

## Egzersiz 3 - Filmler ve Oyuncular
Cem Yılmaz filmlerinde genelde aynı oyuncuların oynadığını fark etmiş olabilirsiniz, bu programda bu konu üzerinde küçük bir inceleme yapacağız.
Cem Yılmaz'ın bazı filmlerini ve bu filmlerin oyuncularını içeren setleri, filmler dictionarysinde görebilirsiniz.

#### Görev 1:
A.R.O.G filminin oyuncu setine Cem Yılmaz'ı yazmayı unuttuğumuzu fark ettik, bu programın ilk görevi bu yanlışlıği düzeltmek.

#### Görev 2:
Bu filmlerde oynayan bütün oyuncuları içeren bir set elde edip, bu oyuncuları konsola yazdıralım.

```bash
#Sonuç

Cem Yılmaz filmlerinde oynayan oyuncuların listesi:
Cengiz Bozkurt
Nil Karaibrahimgil
Özge Özberk
Zafer Algöz
Şafak Sezer
Demet Evgar
Ozan Güven
Rasim Öztekin
Farah Zeynep Abdullah
Tülin Özen
Cem Yılmaz
Özkan Uğur
```
#### Görev 3:
Şimdi de bütün filmlerde oynayan vazgeçilmez oyuncuları bulalım.

```bash
#Sonuç

Cem Yılmaz filmlerinin vaz geçilmezleri:
Ozan Güven
Cem Yılmaz
Özkan Uğur
```

#### Görev 4:
Bütün oyuncuların kaç filmde oynadığını sayalım, ve konsolda gösterelim.

```bash
#Sonuç

Sayı	Oyuncu
1 	 Nil Karaibrahimgil
3 	 Özge Özberk
4 	 Zafer Algöz
5 	 Ozan Güven
5 	 Cem Yılmaz
5 	 Özkan Uğur
1 	 Cengiz Bozkurt
1 	 Tülin Özen
1 	 Demet Evgar
1 	 Farah Zeynep Abdullah
1 	 Şafak Sezer
1 	 Rasim Öztekin
```



## Ekstra 1 - Adam Asmaca
Eskiden arkadaşlarınızla adam asmaca oynadığınız günleri hatırlıyor musunuz? Eskiden kağıt kalemle oynanan bu oyunu gelin beraber bilgisayarda oynanan halini yazalım. Oyunun kuralları şöyle:  

- Listeden seçtiğiniz rastgele bir kelimenin harf sayısı kadar ekrana çizgi çizeceğiz.
- Oyuncunun önceden belirlenen sabit sayıda canı var. 
- Oyuncu her turda bir harf seçer, 
  - Eğer bu harf doğruysa ekranda doğru harfin olduğu yerdeki çizgileri kaldırmamız ve bu harfi koymamız gerekiyor.
  - Eğer bu harf yanlışsa oyuncunun canını azaltmalı ve oyuncuya kaç canı kaldığını söylemelisiniz.
- Oyun, kullanıcın canı biterse veya bütün kelimeyi doğru tahmin ederse, yani ekranda hiç çizgi kalmazsa biter.

```bash
# Örnek Çalışma Şekli 
Adam Asmaca Oyununa hoşgeldin! Kelimeyi doğru tahmin etmek için 3 canın var.
______
> Tahminin: P
P_____
> Tahminin: A
Tahminini yanlış :( 2 canın kaldı.
P_____
> Tahminin: Y
PY____
> Tahminin: O
PY__O_
> Tahminin: T
PYT_O_
> Tahminin: H
PYTHO_
> Tahminin: N
Tebrikler, oyunu kazandın!
```