---
layout: post
title: Final Projesi Sıkça Sorulan Sorular
subtitle: 
categories: final_projesi
authors: [Arda Enfiyeci, Gül Sena Altıntaş]
tags: [final_projesi]
# slug: final-projesi-sss
permalink: /2021bahar/projeler/final-projesi-sss
---
## Uzaylıları oluştururken problem yaşıyorum ne yapmalıyım?
### Tek bir uzaylı görüyorum
Eğer uzaylılarınızı bir for döngüsüyle oluşturuyorsanız büyük ihtimalle uzaylıları aynı x ve y koordinatlarına eklediğiniz için bu hatayla karşılaşıyorsunuz.
Her uzaylı için neyin değiştiğini, x ve y koordinatlarını nasıl belirleyeceğinizi düşünmelisiniz.

### Uzaylıların sadece biri hareket ediyor
Bu problemde uzaylı ve hız listelerinize bakmalısınız. Büyük ihtimalle `uzayli_listesi`'ne tek bir uzaylı ekliyorsunuz. Bu nasıl olabilir, bir örnekle inceleyelim:
Örneğin, 0'dan 2'ye kadar bütün sayıları bir listede tutmak istiyorum. Aşağıdaki üç programı çalıştırırsam sonuçların nasıl olacağını düşünün. Doğru şekli 2. programda.
Siz kodunuzda 1. ve 3. örnekteki hatayı yapıyor olabilir misiniz?
```python
for i in range(3):
    l = list()
    l.append(i)
    print(l)
```

```python
l = list()
for i in range(3):
    l.append(i)
    print(l)
```

```python
l = list()
for i in range(3):
    print(l)
l.append(i)
print(i)
```

- Birinci programın sonucu:
```
[0]
[1]
[2]
```
- İkinci programın sonucu:
```
Sonuç:
[0]
[0, 1]
[0, 1, 2]
```

- Üçüncü programın sonucu:
```
[]
[]
[]
[2]
```
## Uzaylılarımın hepsi aynı yönde hareket ediyor ne yapmalıyım?

Bu problemle karşılaşmanızın sebebi genellikle
hız listesi oluştururken her uzaylı başına bir adet 
hız değeri oluşturulmasıdır. Move fonksiyonu `kanvas.move()` fonksiyonu 3 argüman alır: 
hareket ettireceğimiz obje, x yönündeki hız değeri, y yönündeki hız değeriAncak iki boyutlu bir alanda
çalıştığımız için her vektörün farklı yöne bakabilmesi 
için hem x düzlemi hem de y düzlemi için iki farklı değer 
oluşturmalıyız. Matematikte dikliği nasıl hesapladığımızı
hatırlayalım, önemli olan x ve y değerlerinin birbirlerine
olan orantısı.

![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_1.jpg){: width="350px" }
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_2.jpg){: width="350px" }

Eğer uzaylılarımızın hareketindeki 
x ve y değeri eşit olursa,
birbirlerine olan oranları hep 1 olacaktır ve uzaylılarımızın 
hepsi aynı şekilde yol alıcaktır.
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_3.jpg){: width="350px" }
Bu nedenle hız listesi yapımız şu şekilde olmalıdır:

`[[hiz0_x, hiz0_y], [hiz1_x, hiz1_y], ..., [hizn_x, hizn_y]]`

Aynı zamanda uzaylılarımızın rastgele hareketinin 
360 derece yani her yöne olmasına istiyorsak, hız listemizi
oluştururken MIN hız değerini negatif bir sayı yapabiliriz.

## Uzaylıları oluşturdum, hız_listesi oluşturdum ancak onları nasıl hareket ettirebilirim?

Öncelikle uzaylıları oluştururken onları bir listeye eklediğimizden emin olalım.
Yoksa sonrasında dönüp oluşturduğumuz uzaylıya ulaşmakta zorlanırız.
Hız listemiz ile uzaylı_listemiz aynı uzunlukta olmalı ki böylece
her uzaylı başına düşen bir hızımız var. Bu durumda bir for döngüsü kullanarak amacımıza ulaşabiliriz.

## Uzaylıları nasıl duvardan sektireceğim?

Uzaylıların hareketlerini x ve y'nin birleşimi ile oluşan
bir vektör gibi düşünmenin faydalı olucağını yukarda konuşmuştuk.
Şimdi düşünmemiz gereken şey bu uzaylıların duvara çarptıklarında 
x ve y değerlerinde nasıl bir değişim gerçekleşeceği. Aşağıdaki 
görseller size yardımcı olabilir:
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_4.jpg){: width="350px" }
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_5.jpg){: width="100px" }
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_6.jpg){: width="100px" }
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_7.jpg){: width="350px" }
![](/assets/images/2021bahar/final_project/faq-screenshots/PHOTO_8.jpg){: width="350px" }

Bir objeniin kordinatlarına `get_left_x` ve `get_top_y()` ve fonksiyonları ile 
ulaşabildiğimizi unutmayalım, bu durumda tek yapmamız gereken 
uzaylılarımızın kanvasın sınırlarını değip değmediklerine bakmak 
ve şayet deydilerse değen uzaylının hız değerlerini hız listesinde 
değiştirmek.

***
## SIK YAPILAN HATALAR
 
Zamanla güncellenecektir, başarılar.

