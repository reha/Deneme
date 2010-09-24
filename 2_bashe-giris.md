#2) bash'e Giriş

##Kabuk

Linux komut satırına girdiğinizde aşağıdakine benzer bir komut satırı ile karşılaşırsınız;

`$`

Bunu görüntüleyen programa kabuk (shell) denir. Büyük ihtimalle sisteminiz bash kabuğu ile sizi karşılayacaktır. Bunu kontrol etmek için komut satırına şunu yazınız;

`echo $SHELL`

Ekranda ne çıktı? Eğer [şu](http://unix.reha.us/files/2.1.kabuk_.gif) şekilde bir görüntü ile karşılaştıysanız bash kabuğunu kullanıyorsunuz.

“Bourne-again shell” ifadesi için bir tür kısaltma olan bash, pek çok Linux sisteminde ön tanımlı kabuk olarak karşınıza çıkar. Görevi; Linux sisteminizle etkileşime geçmenizi sağlamaktır. Kabuğun çalışmasını sonlandırmak için şu kombinasyonu kullanabilirsiniz;

`Ctrl + D`

##pwd ve cd

“Print Working Directory”nin kısaltması olan şu komut bize bulunduğumuz dizini gösterir;

`pwd`

“Change Directory”nin kısaltması olan şu komut ise bir dizine gitmemize yarar;

`cd`

cd komutunu kullanarak ana dizine gidiniz ve gittiğiniz yerin ana dizin olduğundan emin olunuz. [Buradaki](http://unix.reha.us/files/2.4.cd-kullan%C4%B1m%C4%B1-2.5-yollar.gif) gibi bir görüntü ile karşılaşacaksınız…

##Mutlak Yollar

Size bir mutlak yol örneği verelim;

`/usr/local/bin`

Mutlak yollar daima / ile başlarlar. Özelliği ana dizinden başlayarak bulunduğu yere kadar yolunu göstermesidir.

##Göreli Yollar

Bağıl yollar da diyebileceğimiz yoldur. Bu tür yollar daima içerisinde bulunan dizine göre yorumlanır. Örneğin aşağıdaki gibi bir yol girildiğinde içinde bulunduğumuz klasörün içindeki local klasörünün içindeki bin klasörü anlaşılacaktır;

`local/bin`

##"."

Şuan bulunduğumuz konum manasına gelir. cd komutunu kullanarak bir dizine gidiniz ve . kullanarak da o dizin içindeki bir dizine gidiniz. [Burada](http://unix.reha.us/files/2.11.-.-kullan%C4%B1m%C4%B1.gif) benzer bir örnek mevcut.

##“..”

Bir üst dizin manasına gelir. Bunu kullanarak bir üst dizindeki bir dizine gidiniz. [Burada](http://unix.reha.us/files/2.8.ciftnoktakullan%C4%B1m%C4%B11.gif) bu işlemin nasıl yapıldığını görebilirsiniz.

##“~”

Tilda karakterini tanıyor musunuz? Bu karakteri Unix’de başka bir kullanıcının dosyalarına erişmek için kullanabiliriz.

`./program ~kullaniciadi/dosya.txt`

##Home dizini

Home dizinine yukarıda gördünüz yollar ile erişmeye çalışınız. Ana dizine giderek cd’nin yanına /home/ ve dizininizin ismini yazmak yeterli olacaktır. Ancak daha kolay bir yol var. O da komut satırına şunu yazıp Enter’a basmak;

`cd`

