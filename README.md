## Ders 3 | Dizinler Arasında Gezme/İçerik Listeleme

[< Anasayfa](https://saricayemre.github.io/linuxkomutsatiridersleri/)

# Giriş

Linux sistemlerde tüm dosyalar bir kök dizine yani root'a bağlıdır. root dizini / (slash) ile ifade edilir. Ayrıca root haricinde her kullanıcının bir home (ev) klasörü mevcuttur. Linux'ta yeni bir terminal açtığınızda, terminaliniz hom klasöründe çalışmaya başlar. Dolayısıyla konsoldan bu dizinlere erişme ve içeriklerini listeleme mümkündür. Bunun haricinde kullanıcıların kendi oluşturmuş olduğu dizinler ve diğer her şey için dizin arasında gezinme ve listeleme işlemi yapmak mümkündür. Şimdi bu komutların neler olduğuna bakalım.

## pwd

O an hangi dizin içinde çalıştığımızı görmek istediğimiz zaman terminale `pwd` komutunu girmemiz yeterli olacaktır. Aslında bunu zaten görsel olarak görebiliyoruz. Ama çoklu kullanıcıların olduğu sistemlerde sistem yöneticisi olduğunuzu düşünün. Hangi kullanıcının nerde olduğunu görmek bu komutla mümkün oluyor.

![pwd-img](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/pwd-img.png?raw=true)

## cd

`cd` komutu ile dizinler arasında gezinme işlemini gerçekleştiriyoruz. Komutu `cd gidilecek_konum` şeklinde kullanırsak sonuca varmış oluruz. Örneğin sistemde var olan /usr/share klasörüne gitmek için, `cd /usr/share` komutunu terminale girmemiz ve çalıştırmamız yeterli olacaktır.

![cd-img1](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/cd-img1.png?raw=true)

İç içe dizinlerin içerisinde olduğumuzu varsayarsak, bulunduğumuz dizinden _bir üst dizine_ gitmek için `cd ..` vaya `cd ../` komutlarından birini kullanmamız yeterlidir. Eğer _iki üst dizine_ gitmek istiyorsak, `cd ../../` komutunu, _üç dizin_ üste gitmek isiyorsak `cd ../../../` komutunu kullanmalıyız. Buna benzer olarak geçeceğiniz dizin sayısını arttırabilirsiniz. Ayrıca _Ana Dizine_ gitmek istediğimizde sadece ` cd` komutunu kullanmak yeterli olacaktır. 

![cd-img2](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/cd-img2.png?raw=true)

## ls

Herhangi bir dizin altında bulunan her şeyi görüntülemek için `ls` komutnu kullanırız. Bu komut sayesinde bir dizinin altında neler olduğunu terminal ekranında görüyoruz. 

![ls-img1](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/ls-img1.png?raw=true)

Eğer dizin altındaki dizin ve dosyalar hakkında detaylı bilgi almak yani okuma, yazma, çalıştıma, oluşturma tarihi vs gibi detaylı bir bilgi için `ls -l` komutunu kullanmak gerekir. 

![ls-img2](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/ls-img2.png?raw=true)

Ayrıca gizli dosyaları da görüntüleyebiliriz. Bunun için `ls -la` komutunu kullanırız. 

![ls-img3](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/ls-img3.png?raw=true)

## Tarayıcıdan Dizin Yapısına Erişmek

Lİnux sistemlerde web tarayıcılardan dosya ve dizinlere erişmek mümkündür. Bunun için web tarayıcısını açıp adres çubuğuna `/` yazıp enter'a basmanız yeterlidir. Karşımıza root dizininin yapısı çıkacaktır. Burada mouse yardımıyla dizinlerin altında neler olduğunu görebiliriz. 

![web-img1](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/web-img1.png?raw=true)

Web tarayıcıda dizinler arasında adres çubuğu ile ilerlemek mümkündür. _cd_ komutunda anlattığım `../` ifadeleri burda adres satırına girildiğinde bir üst satıra gidebilirsiniz. Diğer parametrelerde aynı şekilde geçerli olacaktır. 

Son olarak, adres çubuğuna `man:cat` yazdığımızda man kılavuz sayfasını görüntüleyebiliyoruz. Man kılavuz sayfası, yardım alma komutlarının tutulduu yerlerdir.

![web-img2](https://github.com/saricayemre/linuxkomutsatiridersleri-ders3/blob/main/resimler/web-img2.png?raw=true)

## Ders Sonu

Bu dersimizde Linux dizinleri arasında gezinmeyi ve içeriklerini listelemeyi öğrenmiş olduk. Bu komutları sizlerde çalıştırarak hepsinin uygulamasını yaparsanız ve ilerleyen derslerimizde kullandığımızda ne anlama geldiğini hemen hatırlayacak ve unutmazsınız. :)

[< Önceki Sayfa](https://saricayemre.github.io/linuxkomutsatiridersleri-ders2/) | [Sonraki Sayfa >](https://saricayemre.github.io/linuxkomutsatiridersleri-ders4/)
