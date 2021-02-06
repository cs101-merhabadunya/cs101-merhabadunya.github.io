---
layout: post
title: Hafta 8 - Grup Çalışması Egzersizleri
subtitle: İnternetten Veri Kazıma
categories: grup çalışması
authors: [Gül Sena Altıntaş, Ozan Nacitarhan]
tags: [grup çalışması]
slug: hafta8-grup
---

## Başlangıç Kodları

[Buraya tıklayarak](https://drive.google.com/file/d/1__TX9mRsjZHVREKYJIN1KiIQG7Qguy0X/view?usp=sharing) bu haftaya ait çalışmaların başlangıç kodlarına ulaşabilirsiniz. Dilerseniz [Ed üzerinden](https://us.edstem.org/courses/2639/lessons/7683/edit/slides/37118) de çalışabilirsiniz.


## Ön Bilgi
Günlük hayatta olduğu gibi internetteki iletişimin de kuralları var. Web tarayıcımız ile web server'u arasında iletişim kurmamızı 
sağlayan kural ve metodları *protokol* olarak adlandırıyoruz. Bu haftaki egzersizimizde HTTP Protokolüne ait metodları kullanacağız. 
Meraklısı [buradaki](https://www.hosting.com.tr/bilgi-bankasi/http-nedir/) gibi bir kaynaktan daha fazla bilgi edinebilir.

HTTP (Hyper Text Transfer Protocol)'de en çok kullandığımız metodlar şöyle:

| HTTP Metodları | Açıklamaları | Örnek |
|:--------------:|:------------ |:------|
| GET   | Get metodu ile bir sorgu gerçekleştirebilir ve sonucunu sunucudan elde edilebilir. | Arama, Belge indirme |
| HEAD  | Head GET ile aynı işlemi yapar ancak yanıtta gövdeyi istemez. | - |
| POST  | Post ile sunucuya veri veya bir komut gönderebiliriz, genellikle sunucuda bir durum değişikliği yaratır. | Sitenizdeki bir veriyi güncellemek, medya aktarmak |
| DELETE| Mesajda belirtilen kaynağı siler. | Gönderi silmek, kaldırmak |
 
Diğer HTTP metodlarına [bu siteden](https://developer.mozilla.org/tr/docs/Web/HTTP/metotlar) bakabilirsiniz.

## Ön Hazırlık
### Python requests kütüphanesi
Bu haftaki egzersizlerimiz için `requests` kütüphanesini ve `BeautifulSoup` kullanacağız, onun için `terminale aşağıdaki komutu yazarak requests ve BeautifulSoup kütüphanelerini indirin:  
```commandline
python -m pip install requests
python -m pip install beautifulsoup4
```

### Başlamadan Önce
Bir websitesine sorgu yapmak için requests kütüphanesinin `request` isimli fonksiyonunu kullanabiliriz. Buradaki headers, 
ikinci egzersizimizde önemli olacak. Örneğin:  
```python
requests.request('GET', URL, headers=detaylar)
```  
kullanarak belirtilen `URL` adresine gerekli detayları içeren (API anahtarı gibi) bir `GET` isteği gönderebiliriz. Denemek için
```python
response=requests.request("GET", "https://cs101-merhabadunya.github.io/hakkimizda")
```

Aldığımız cevabı (response) inceleyelim:
- Cevabın statüsü `response.status_code`  
Eğer 200 ise sorgumuz başarıyla gerçekleştirildiği, 403 ise sağladığınız API anahtarında bir hata olduğu anlamına gelir. 403 cevabı aldığınızda api anahtarınızı kontrol kedin. 
- Sorgumuzun microsaniye cinsinden ne kadar sürede cevaplandığı: `response.elapsed`
- Sorgumuzda kullanılan url: `response.url`
- Cevapta bize iletilen text (yazı): `response.text`

Cevabı aldıktan sonra, BeautifulSoup kütüphanesinin kendi fonksiyonlarını kullanarak websitesinin istediğiniz kısmındaki bilgilere ulaşabilirsiniz. class-adi olan yere istediğiniz class'ı yazıp oradaki bilgiyi alabilirsiniz.
```python
soup = BeautifulSoup(response.content, "html.parser")
aradigimiz_yer = soup.find("div", attrs={"class":"class_adi"})
yazi = aradigimiz_yer.text
```

Tarayıcımızda bir internet sayfasına girdiğimizde sağ tıklayıp "İncele" (Inspect) seçeneğine bastığımızda sayfanın html koduna ulaşabiliyoruz. 
Sayfanın html koduna ulaştıktan sonra da açılan pencerede (genelde kutunun üzerinde bir mouse imleci olarak gözükür) 
incelenecek bir element seç butonuna basıyoruz. Bu butona bastıktan sonra anlık kurun üzerine gelip tıkladığımızda bize onun html kodundaki yerini gösterecektir. 
Buradaki `class, id` gibi özellikleri kullanarak BeautifulSoup'da kolay filtreleme yapabiliriz.
Aşağıdaki ekran görüntüsünde bir örneğini görebilirsiniz:
![Chrome'da html kodu inceleme](/assets/images/sections/week8/chrome-inspect.jpeg)

## Egzersiz 1
Hızla globalleşen günümüz dünyasında artık saniyelerin bile çok önemi var. Para birimlerinin değerleri saniyeler içinde değişebiliyor. Sizden anlık olarak para değerlerini alıp, 
güncel kura göre dönüşüm yapabilen bir kod yazmanızı istiyoruz.

Bu egzersizimizde [doviz.com](https://kur.doviz.com/serbest-piyasa) sitesinde olan güncel döviz kurlarından yararlanacağız.

### Döviz kurları
Döviz kurlarının güncel olması için, kodumuz her çalıştığında döviz kurlarını tekrar almamız gerekiyor. Dolar kurunu almak için bu [linkteki](https://kur.doviz.com/serbest-piyasa/amerikan-dolari), 
Euro kurunu almak için de bu [linkteki](https://kur.doviz.com/serbest-piyasa/euro) sayfayı kullanıyor olacağız. Ön bilgi bölümünde anlatıldığı 
gibi sayfanın HTML kodunu açıp buraki class isimlerini ve BeautifulSoup kütüphanesini kullanarak anlık döviz kurunu alalım.

### Kur dönüşümü yapma
Kullanıcıya hangi kurdan hangi kura çevirmek istediğini ve ne kadar miktar parayı dönüştürmek istediğini soralım. Sonrasında gerekli matematik işlemini yaparak kullanıcıya sonucu gösterelim. 

Örnek Çıktı:
```
Hangi para birimlerini dönüştürmek istiyorsunuz? usd-try
Kaç USD'nin TRY karşılığını merak ediyorsunuz? 1000
1000.0 $ = 7670.9 TRY
```

## Egzersiz 2
Bu haftaki CS 101 ekip toplantısında karantina bitse de eskisi gibi sokaklarda özgürce yürüyebilsek sinemaya, kafelere, lokantalara gidebilsek gibi dilekler dile getirildi. 
Eğitmenlerinin bu dileklerine CS 101 öğrencilerinin sessiz kalmayacağını düşündük. İyi birer programlamacı olarak sizden 
CS 101 eğitmenlerinin karantina bitiminde gidebilecekleri restoranları bulmanızı istiyoruz.

Bu egzersizimizde [Zomato'nun](https://www.zomato.com/tr/istanbul) geliştiriciler için sağladığı API'yi kullanarak şu sorulara cevap bulacağız:

### Ön hazırlık
#### API anahtarı oluşturalım
API kullandığımızda çoğunlukla servislerini kullanacağımız siteden bir anahtar üretmemiz gerekir. Bu anahtarı site ile 
tüm iletişimimizde (istek atmak, bilgi edinmek, vb.) kullanırız ve bu sayede site bizim yaptığımız işlemlerin takibini tutabilir.
Aynı zamanda site bizim apiyi kullanma miktarımızı ticari ve yasal sebeplerle sınırlayabilir. Bir API kullanırken sitenin
kullanım koşullarını dikkatle incelememiz önemli!

Bu sebeple, önce Zomato'nun geliştiriciler için hazırladığı siteye girerek anahtar edineceğiz. [Bu siteden](https://developers.zomato.com/api?lang=tr#headline2)
giriş yaparak `API anahtarı oluştur` butonuna tıklayarak anahtarımızı üretebiliriz. Anahtarınız günlük maksimum 1000 çağrı
yapmanıza izin veriyor.

#### Zomato API'si Dokümantasyonu
Zomato API'sinin dokümantasyonuna [buradan](https://developers.zomato.com/documentation?lang=tr#!/) ulaşabilirsiniz.
Fark ettiyseniz Zomato API'si ile kullanabildiğimiz tek HTTP metodu `GET` bu demek oluyor ki bu API ile sadece bilgi isteyebiliriz ve 
sunucuda değişiklik yapamayız.

### Görevler
Burada sorgudan gelen cevapların formatı api'ye bağlıdır. Bu sebeple size verdiğimiz 
`get_sorgusu_cevabi` fonksiyonunu kulanabilirsiniz, bu fonksiyon cevabı bir 
dictionary olarak döndürür. Bu fonksiyondan aldığınız değeri konsola yazdırarak dictionary'nin formatı, anahtarları ve içerdiği değerlerle ilgili daha çok bilgi edinebilir ya da dönen cevabın formatını Zomato'nun Dokümantasyonundaki örneklerden de inceleyebilirsiniz.

#### Kategoriler
<span>1.</span> Hasan Can seçenekleri görmek için önce Zomato'daki bütün kategorileri bulmak istiyor. Bunun için 'GET' 
kullanarak `api_baz_url` olarak verilen url'ye "/categories" stringini ekleyerek request oluşturmalıyız. 
`get_sorgusu_cevabi` fonksiyonunu kulanabilirsiniz. Ancak formatın daha kompakt bir şekilde tutmak isteyen Hasan Can Fırat'tan yardım ister ve gelen sonucu {id_1: isim_1, id_2: isim_2} gibi bir dictionary'de tutmasını rica eder. Fırat'a yardım edelim.

Örnek Çıktı:  
```
{1: 'Delivery', 2: 'Dine-out', 3: 'Nightlife', 4: 'Catching-up', 5: 'Takeaway', 6: 'Cafes', 7: 'Daily Menus', 8: 'Breakfast', 9: 'Lunch', 10: 'Dinner', 11: 'Pubs & Bars', 13: 'Pocket Friendly Delivery', 14: 'Clubs & Lounges'}
```

#### Şehirler
<span>2.</span> Gül Sena Zomato'yu Balıkesir'de de kullanıp kullanamayacağını öğrenmek istiyor. `"https://developers.zomato.com/api/v2.1/cities?q=SEHIR"`
url'sini kullanarak Balıkesir'deki restoranlarla ilgili bir bilgi olup olmadığını bulalım. Sorgunun sonucunda dönen dictionary'deki
`'has total'` anahtarının değerini kullanabiliriz.

Örnek Çıktı:  
```
Üzgünüm Gül Sena, Balıkesir'deki lokantalarla ilgili bir bilgim yok.
```

<span>3.</span> Balıkesir'deki restoranlarla ilgili bilgi edinemeyen Gül Sena'yı teselli etmek isteyen İdil ve Oya 
İstanbul'da hangi mutfaklardaki restoranların olduğunu bulmak isterler ve aralarında iş bölümü yaparlar. 
- İdil `"/cuisines"` anahtar kelimesini kullanabileceklerini fark eder ancak bu sorgu için `city_id`si (şehir kimliği) bilgisine 
ihtiyaç duyduklarını fark eder. 
- Oya `"/cities"` anahtar kelimesini kullanarak İstanbul'un bilgilerine ulaşmalı ve `city_id`sini bulmalıdır.
Oya'ya yardım etmek için `get_sorgusu_cevabi` fonksiyonunu kulanabilirsiniz. 
Bu bilgiyi elde edebileceğimiz url şu şekilde: `https://developers.zomato.com/api/v2.1/cities?q=ISTANBUL`
Bu sorgu sonucunda dönen dictionary'de 'location_suggestions' anahtarının değerinini incelemelisiniz.
- Daha sonra İdil bu id'yi kullanarak İstanbul'daki mutfak türlerini bulabilir. Yine `get_sorgusu_cevabi` fonksiyonunu kullanabilirsiniz. 
Bu bilgiyi elde edebileceğimiz url şu şekilde olacaktır: `https://developers.zomato.com/api/v2.1/cuisines?city_id=SEHIR_IDSI`

Örnek Çıktı:  
```
Oya: İdil, İstanbul'un şehir id'si 59
İdil: Teşekkürler Oya!
İdil: Gül Sena! İstanbulda toplamda 69 mutfak var, aşağıda bütün mutfakları görebilirsin: 
{171: 'Aegean', 1: 'American', 4: 'Arabian', 3: 'Asian', 5: 'Bakery', 341: 'Balkans', 227: 'Bar Food', 132: 'Belgian', 270: 'Beverages', 170: 'Black Sea', 133: 'British', 168: 'Burger', 351: 'Börek', 30: 'Cafe', 172: 'Central Anatolia', 202: 'Central Asian', 25: 'Chinese', 1040: 'Coffee', 100: 'Desserts', 268: 'Drinks Only', 721: 'Döner', 174: 'Eastern Anatolia', 38: 'European', 40: 'Fast Food', 271: 'Finger Food', 45: 'French', 187: 'Fresh Fish', 134: 'German', 180: 'Giblets', 156: 'Greek', 181: 'Grill', 521: 'Hawaiian', 143: 'Healthy Food', 169: 'Home-made', 233: 'Ice Cream', 148: 'Indian', 140: 'Iranian', 55: 'Italian', 310: 'Izgara', 60: 'Japanese', 164: 'Juices', 178: 'Kebab', 1056: 'Kokoreç', 67: 'Korean', 711: 'Kumpir', 66: 'Lebanese', 70: 'Mediterranean', 73: 'Mexican', 137: 'Middle Eastern', 184: 'Old Turkish Bars', 176: 'Ottoman', 306: 'Pastry', 183: 'Patisserie', 1004: 'Pilav', 82: 'Pizza', 1017: 'Restaurant Cafe', 1005: 'Roast Chicken', 84: 'Russian', 83: 'Seafood', 173: 'South East', 89: 'Spanish', 141: 'Steak', 177: 'Sushi', 163: 'Tea', 95: 'Thai', 142: 'Turkish', 186: 'Turkish Pizza', 185: 'World Cuisine', 262: 'Çiğ Köfte'}
```  

#### Lokanta Aramak
<span>4.</span> Bunu duyan Ahmet, evini özlediğini söyleyip Ege mutfağından bir lokantaya gitmek ister ve Demet'in yardımını rica eder. Demet
`"/search"` anahtar kelimesini kullanarak İstanbul'daki Ege mutfağı (Agean) restoranlarını aramalı ve fiyatlarına (cost) göre bunları 
sıralamadır. Ozan başka bir sorguda bu url'yi kullandığını söyler: `"https://developers.zomato.com/api/v2.1/search?entity_id=59&entity_type=city&cuisines=70&category=delivery&sort=rating&order=asc"`
Ozan'ın url'sini değiştirerek Demet'e yardımcı olalım. İpucu: Ege mutfağının id'si 171 ancak bu bilgiyi İdil'in bir önceki
aşamada bulduğu dictionary'den de elde etmeyi deneyebilirsiniz

Örnek Çıktı:
```
Ahmet: Evimi özlediim.
Demet: Merak etme Ahmet, 46 kadar lokanta buldum
Demet: Yekta, gideceğimiz restoranın id'si: 18305691
```

#### Restoran Detayları
Yekta Demet'in sorgusunda bulduğu birinci restoranın id'sini öğrenir ve `"https://developers.zomato.com/api/v2.1/restaurant?res_id="` url'sini kullanarak restoran hakkındaki detayları inceler. Restoranın adresini
Necla'ya verir. Karantina bittiğinde Ahmet (diğeri) Necla'nın başka bir API kullanarak bulduğu navigasyon bilgileri ile ekibi restorana götürür. Ancak bir süre
daha evde kalmamız doğru olacağı için bu son işlemi ileriye bırakıyoruz. Kim bilir, belki de CS 101 Bahar 2021 dönemi öğrencileri
de bu görevi tamamlar :).

Örnek Çıktı:
```
Yekta: Necla, gideceğimiz restoranın adresi: Ömer Avni Mahallesi, İnönü Caddesi, No 26, Kat 8, Beşiktaş, İstanbul
```

Herkese afiyet olsun!
