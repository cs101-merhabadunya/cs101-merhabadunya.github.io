---
layout: post
title: Hafta 7 - Grup Çalışması Egzersizleri
subtitle: Teachable Machine
categories: grup çalışması
authors: [Gül Sena Altıntaş, Oya Sura]
tags: [grup çalışması]
slug: hafta7-grup
---

## Başlangıç Kodları

Bu haftaki çalışmalarımızı Tensorflow kütüphanesini kullanacağız. Ancak Tensorflow kütüphanesi kullanmaya alışık olduğumuz kütüphanelere göre daha çok hata verebileceği ve yüklemesi zor olduğu için bu hafta Repl.it isimli online IDE'den faydalanacağız. Lütfen kendinize bir [Repl.it](https://repl.it/) hesabı açın. 

[Buraya tıklayarak](https://repl.it/@gsaltintas/CS101-Grup-Calismasi-7) bu haftaya ait çalışmaların başlangıç kodlarına ulaşabilirsiniz.
<iframe height="400px" width="100%" src="https://repl.it/@gsaltintas/CS101-Grup-Calismasi-7?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Makine Öğrenmesi
Yapay zekanın bir alt başlığı olan Makine Öğrenmesi bilgisayar bilimcilerin çok uzun zamandır çalıştığı bir konu. Makine öğrenmesi kast ettiğimiz aslında belli görevleri otomize edebilen veya karşılaştığı koşullara göre karar alabilen programlar tasarlamak. Örneğin bir çocuk nasıl el yazısı yazmayı öğreniyorsa benzer şekilde bir makine de el yazısı yazmayı öğrenebilir. Burada önemli olan istenilen görevlerin açık ve net bir şekilde kararlaştırılması, doğru matematiksel modellemesinin yapılması ve kaliteli bir veri seti ile bu sürecin makineye *öğretilmesi*dir. 

## Egzersiz
Bu çalışmada Yelda'ya yardım etmeye çalışıyoruz. Yelda daha 3 yaşında oluduğu için hayvanlar arasındaki farklıları bilmiyor mesela dört ayaklı ve tüye sahip her hayvana kedi diyor. Bu sebepten Yelda'ya iki farklı hayvan örneği gösterip (kedi ve köpek) hayvanları belirli ölçüde ayırt etmesini sağlamaya çalışıyoruz. 

Size verilen kodda Yelda'ya öğretmek için kullandığımız bir veri topluluğu var. Biz bu kısmını derste gördüğümüz TeachableMachine ile hallettik sizden şunları bekliyoruz:

1. Yelda'ya diğer örnek canlıları gösterip onun tahminini almak (Bunun için biz tahmin fonksiyonu verdik)

2. Bu tahmine göre hayvanlar sözlüğündeki tahminin ait olduğu hayvanın değerini artırmak.

3. Son olarak da bu hayvanın fotoğrafını Yelda'nın odasındaki kanvasa yapıştırmasını sağlamak.

### Meraklısına
Bu egzersizde Google'n TeachableMachine'ı kullanılarak sınıf tanıma modeli eğitilmiştir. Eğitim için kullanılan resimler Kaggle'daki [Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats/data) Challenge'nda yayınlanan 25 bin fotoğrafın bir bölümünü kapsamaktadır. Modelin eğitimi sırasında kullanılan parametreler:
- Eğitim için her sınıf başına 60 resim
- Epoch: 50, Batch size: 16, learning rate: 0.001

### Bonus
Projemizi ilerletebileceğiniz noktalar:
1. Yelda'nın hayvanları hatırlamasına yardımcı olmak için kanvasa eklediğiniz her fotoğrafın altına hayvanın türünü ekleyebilirsiniz.
2. Modelimizin doğruluk oranını ölçümlemek