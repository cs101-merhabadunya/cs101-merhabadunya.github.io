---
layout: post
title: PyCharm Kurulumu
permalink: /pycharm-python/
authors: [Demet Tümkaya]
categories: planlama
tags: [planlama, kod]
---

**CS 101: Merhaba, dünya!** programı boyunca, bilgisayarınızda kodu yazmak, çalıştırmak, incelemek ve hata ayıklamak için PyCharm adı verilen bir uygulama kullanıyor olacaksınız. PyCharm, *IDE* yani Bütünleşik Geliştirme Ortamı (Integrated Development Environment) türünde bir uygulamadır ve yaygın olarak kullanılmaktadır. Bu doküman sizlere kurulumun nasıl yapılacağını anlatmak için oluşturulmuştur.

## Python’u indirmek
Bilgisayarınızda Python programlarını çalıştırmak için öncelikle bir Python Interpreter indirmelisiniz, bu PyCharm’ın varlığına bağlı bir durum değildir.
    
Interpreter adı verilen yorumlayıcı programlar, `.py` uzantılı dosyaları okuyarak kodunuzu bilgisayarınızın işleyebileceği hale getirir. Python’un farklı versiyonları bulunmaktadır, bu program süresince **Python 3.8** kullanacağız. 

>İndirmek için aşağıdaki linkleri kullanabilirsiniz: 
>* Eğer *Windows* kullanıyorsanız, <a href="https://www.python.org/ftp/python/3.8.6/python-3.8.6-amd64.exe" target="_blank">bu link</a> direkt olarak dosyayı bilgisayarınıza indirecektir.
>* Eğer *Mac* kullanıyorsanız, <a href="https://www.python.org/ftp/python/3.8.6/python-3.8.6-macosx10.9.pkg" target="_blank">bu link</a> ile  gerekli dosyalar indirilecektir.
    
#### Windows için Uyarı
İndirilen dosyayı açtıktan sonra, Python kurulum aşamalarında karşınıza çıkacak "Add Python 3.8 in PATH" seçeneğini işaretlediğinizden emin olun lütfen. 
    
## PyCharm’ı indirmek
PyCharm Community versiyonunu, *Windows* bilgisayarınıza indirmek için <a href="https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC" target="_blank">bu linki</a>, *Mac* bilgisayarınıza indirmek için <a href="https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=mac&code=PCC" target="_blank">bu linki</a> kullanabilirsiniz.

İndirme tamamlandıktan sonra *Windows* için *.exe* uzantılı, *Mac* için ise *.dmg* uzantılı dosyayı açarak varsayılan ayarlarla, yani herhangi bir değişiklik yapmadan ilerleyin ve kurulumu tamamlayın.

## PyCharm’ı kullanıma hazırlamak 
>**NOT:** Görünümler aynı olmasa da hem Mac hem de Windows için aşağıdaki adımları takip edebilirsiniz.
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

