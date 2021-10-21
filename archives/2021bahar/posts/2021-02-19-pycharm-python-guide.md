---
layout: post
title: PyCharm Kurulumu
permalink: /kaynaklar/pycharm-python/
authors: [Demet Tümkaya, Gül Sena Altıntaş]
categories: planlama
tags: [planlama, kod]
---

_CS 101: Merhaba, dünya!_  programı boyunca, bilgisayarınızda kodu yazmak, çalıştırmak, incelemek ve hata ayıklamak için PyCharm adı verilen bir uygulama kullanıyor olacaksınız. PyCharm, *IDE*  yani Bütünleşik Geliştirme Ortamı (Integrated Development Environment) türünde bir uygulamadır ve yaygın olarak kullanılmaktadır. Bu doküman sizlere kurulumun nasıl yapılacağını anlatmak için oluşturulmuştur.

## Python’u indirmek
Bilgisayarınızda Python programlarını çalıştırmak için öncelikle bir Python Interpreter indirmelisiniz, bu PyCharm’ın varlığına bağlı bir durum değildir.
    
Interpreter adı verilen yorumlayıcı programlar, `.py` uzantılı dosyaları okuyarak kodunuzu bilgisayarınızın işleyebileceği hale getirir. Python’un farklı versiyonları bulunmaktadır, bu program süresince **Python 3.8** kullanacağız. 

>İndirmek için aşağıdaki linkleri kullanabilirsiniz: 
>* Eğer *Windows* kullanıyorsanız, <a href="https://www.python.org/ftp/python/3.8.6/python-3.8.6-amd64.exe" target="_blank">bu link</a> direkt olarak dosyayı bilgisayarınıza indirecektir. Bilgisayarınız 32bit ise <a href="https://www.python.org/ftp/python/3.8.6/python-3.8.6.exe" target="_blank">bu linki</a> kullanmalısınız.
>* Eğer *Mac* kullanıyorsanız, <a href="https://www.python.org/ftp/python/3.8.6/python-3.8.6-macosx10.9.pkg" target="_blank">bu link</a> ile  gerekli dosyalar indirilecektir.
    
#### Windows için Uyarı
İndirilen dosyayı açtıktan sonra, Python kurulum aşamalarında karşınıza çıkacak "Add Python 3.8 in PATH" seçeneğini işaretlediğinizden emin olun lütfen. 
    
## PyCharm’ı indirmek
PyCharm Community versiyonunu, *Windows* bilgisayarınıza indirmek için <a href="https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC" target="_blank">bu linki</a>, *Mac* bilgisayarınıza indirmek için <a href="https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=mac&code=PCC" target="_blank">bu linki</a> kullanabilirsiniz. Eğer bilgisayarınızda 64 bitlik PyCharm hata veriyorsa <a href="https://download.jetbrains.com/python/pycharm-community-2018.3.7.exe" target="_blank">bu linkteki</a> versiyonu indirmeyi deneyebilirsiniz.

İndirme tamamlandıktan sonra *Windows* için *.exe* uzantılı, *Mac* için ise *.dmg* uzantılı dosyayı açarak varsayılan ayarlarla, yani herhangi bir değişiklik yapmadan ilerleyin ve kurulumu tamamlayın.

## PyCharm’ı kullanıma hazırlamak 
>**NOT:**  Bu doküman Eylül 2020'de hazırlandığı için sizin indirdiğiniz PyCharm daha üst bir versiyon olabilir ve sizin bilgisayarınızda aşağıdaki ekran görüntülerinden farklılık olabilir. Görünümler aynı olmasa da hem Mac hem de Windows için aşağıdaki adımları takip edebilirsiniz.
Kurulum tamamlandıktan sonra, programı çalıştırmakla başlayın. 

Program açılır açılmaz karşınıza aşağıdaki gibi bir giriş ekranı çıkacaktır. 

<!-- ![PyCharm Welcome](https://drive.google.com/uc?export=view&id=1Evv8zeAVZREv97g0mVB7bJqbPoTijOkX) -->
![PyCharm Welcome](/assets/images/pycharm-python/p1.png)

Sağ altta bulunan “Configure” listesinden “Settings”i seçerek PyCharm ayarlarını açın.

<!-- ![PyCharm Settings](https://drive.google.com/uc?export=view&id=1YZdkCnmw9tdbgtPDNdzTdjsVWCYm1x1A) -->
![PyCharm Settings](/assets/images/pycharm-python/p2.png)

Ayarlar penceresindeki listeden *Python Interpreter* veya *Project Interpreter*'a tıklayın. Açılan pencerede **“No Interpreter”** yazan açılır listeden **“Show All**” seçeneğini seçin. *(Bilgisayarınızdaki Python versiyonlarına bağlı olarak görünüm resimdekinden farklı olabilir, bu bir sorun değil, “Show All” ile devam etmeniz yeterli.)*

<!-- ![Interpreter](https://drive.google.com/uc?export=view&id=1YTYYa5jkuwloRArcV97OFAo4QXuijJHR) -->
![Interpreter](/assets/images/pycharm-python/p3.png)

Bir sonraki ekranda, **+** işaretine basın.

<!-- ![Add New Interpreter](https://drive.google.com/uc?export=view&id=1yLaOkXhZBtBR-uxIuZleLEkQ4V4FNLOU) -->
![Add New Interpreter](/assets/images/pycharm-python/p4.png)

Yan taraftaki listeden **“System Interpreter”** seçin ve Interpreter ifadesinin yanındaki açılır listeden indirdiğiniz Python versiyonunu (sizler için *Python 3.8* ile başlayan) seçin.

<!-- ![System Interpreter](https://drive.google.com/uc?export=view&id=1a8A0E-ZnUv0FnxBGYcg3GjXpIWS07G1r) -->
![System Interpreter](/assets/images/pycharm-python/p5.png)

Sonrasında aşağıdaki gibi bir görünüme sahip olmalısınız, henüz özel paketler indirmediğiniz için *Package* listesi altında daha az veya farklı isimlerle karşılaşabilirsiniz.

<!-- ![OK](https://drive.google.com/uc?export=view&id=1RLXyEJ6904Wq6e1y9sNQrtgb-UkQA59L) -->
![OK](/assets/images/pycharm-python/p6.png)

Sağ alttaki **OK** butonuna basarak kurulumu ve hazırlığı tamamlayın, artık **Python kodlarınızı yazmaya başlayabilirsiniz!**

## Kurulumunuzu kontrol edin
Python ve PyCharm'ı kurdunuz, kurulumda bir hata olmadığından emin olmak için son bir aşama tamamlayacağız.

Program boyunca PyCharmda projelerinizi açarken çalıştıracağımız _.py_ uzantılı python dosyasını içeren klasörü açmak işimizi çok kolaylaştıracak. Bunun için size önerimiz bir _CS101_ klasörü oluşturmanız ve programla ilgili kodları hafta hafta bu klasörün içinde kullanmanız. Örneğin, benim bilgisayarımda cs101 isimli bir klasör var. Kurulumu denemek için:
- cs101hafta0.zip isimli klasörü bilgisayarıma indirdim. Klasöre [buradan](https://drive.google.com/file/d/1UqrusTPOkYt6LVF52UVgDkoUm1p_KiE1/view?usp=sharing) ulaşabilirsiniz.
- Klasördeki kodu kullanabilmek için arşivden çıkarmam (unzip) gerek. Benim Windows bilgisayarımda .zip uzantılı bir dosyanın üzerine tıkladığımda yukarıda _Ayıkla_ isimli sekmeye tıklayıp _Tümünü Ayıkla_'ya basıyorum. Aynı şeşkilde klasörün üzerine sağ tıklayınca da benzer bir seçenek çıkıyor.
- Ayıklama işlemi bittiğinde .zip uzantısı olmadan aynı isimde bir klasör oluştu. Bu klasörü PyCharm'da açacağım.
- PyCharm'da _File_ menüsünden _Open_'ı seçiyorum. Açılan pencerede bir önceki aşamada ayıkladığım klasörün içindeki `cs101hafta0` isimli klasörü seçeceğim. (PyCharm'da çalıştıracağımız python dosyaalrını direkt içeren klasörü seçmemiz gerekli.) 
- Artık PyCharm'da klasörü açtığıma göre programı çalıştıracağım. Bunun için ekran görüntüsünde olduğu gibi PyCharm'da aşağıdaki bölümden _Terminal_'e tıklıyorum. ![Terminal](/assets/images/pycharm-python/pycharm-terminal.jpg)
- Terminale `python lec1.py` (Mac için `python3 lec1.py`) yazıp Enter'a basın. 
- Program size aşağıdaki gibi bir karşılık verdiyse kurulumunuzu başarıyla tamamladınız demektir! Dilerseniz yaşınızı da girip Enter'a basarak programımızdan doğum yılınızı teyit edebilirsiniz.
```
Python kurulumun doğru, tebrikler!
Kaç yaşındasınız? 
```
Eğer program başka bir sonuç verdiyse önce [Ed](https://edstem.org/us/courses/4754/discussion/)'e bakmanı öneriyoruz, belki yaşadığın sorun hakkında daha önceden bir çözüm sunulmuş olabilir. Eğer Ed'de daha önce cevaplanmadıysa lütfen aldığın mesajın ya da yaşadığın sorunun ekran görüntüsünü bizimle Ed üzerinden yeni bir soru oluşturarak paylaş.  
