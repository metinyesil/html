# HTML Kullanımı, Sıkça Kullanılan HTML Tagları ve Alabileceği Değerler

Test edeceğiniz ve kullanımını sağlayacağınız ortam sizlerin öğrenme hızını arttıracaktır. 

Online Olarak Test İçin: https://www.w3schools.com/html/tryit.asp?filename=tryhtml_basic

Program olarak Test için (Önerim): Sublime Text

---

### Neden Sublime Text?

Çünkü, kod yazarken örneğin bir div'i kapatmanız gerektiğinde bunları sizin yerinize halledecektir. İlk işiniz nasıl işlediğini çözmek. Daha sonrasında kullandığınız editörü değiştirebilirsiniz fakat ilk kullanım için sublime text sizlerin işini görecektir.

İndir: https://www.sublimetext.com/3

---

## HTML Başlangıç sayfası

Aşağıdaki kurallara uyarak yazmanız gerekmiyor fakat her şeye daha kolay hakim olabilmek için bu şekilde yazmanız daha iyidir. Böyle başlarsanız, böyle devam edersiniz.

Örnek Basit HTML Sayfası:
```
<html>
<head>
// Head: Clean Code yazımına göre Title ve CSS kullanımlarının bulunabileceği alandır. 
</head>
<body>
// Body: Sayfa içerisinde bulunabilecek tüm kodların bulunacağı alandır. 
// Not: Javascript kütüphaneleri </body> tagından hemen önce kullanılmalıdır. 
</body>
</html>
```
---

## title Tagı

Sayfa başlığını belirler. Kullanımı basitçe şu şekildedir:

`<title> Başlık </title>`

---

## span, p, b, i, a Tagları

Teker teker basitçe anlatmak gerekirse;

- Düz Yazı Stilleri

`<span>Yazı</span>` - Hiçbir stil eklenmesi yapılmadan düz bir biçimde yazı yazmanızı sağlayan tag. Bu tagın verilmesinin sebebi, sadece bu yazıya stil vermek isterseniz, bunu gerçekleştirebilmenizdir.

`<p> Başlık </p>` - Span tagı ile aynı işlevi görmektedir. Arasındaki tek fark, p tagı yazının altına bir satır boşluk bıraktırır. Span tagının altına br kodu kullanmak gibi.

- Basit Yazı Stilleri

`<b> Başlık </b>` - İçerisindeki yazıyı kalınlaştırmanızı sağlayan tag. 

`<i> Başlık </i>` - İçerisindeki yazıyı italikleştirmenizi (eğik yazmanızı) sağlayan tag.

- Link (a) Tagı

`<a href="https://google.com" target="_blank">Test</a>` - Bu tag bize Test adında, altı çizili mavi bir yazı verecektir. Tıkladığımızda Google'a yönlendirecektir.
target içerisindeki blank özelliği ise bu bağlantıyı yeni sekmede açmamızı sağlar. Dilerseniz kullanmayabilirsiniz.

---

## h1-h6 Tagları

Yazı boyut taglarıdır. Bu taglar, belirli font büyüklükleriyle yazı yazmanızı sağlar. Aşağıdaki şekilde kullanılmaktadır. En büyük yazı h1, en küçük yazı h6 tagıdır.

`<h1>Yazı</h1>`
`<h2>Yazı</h2>`
`<h3>Yazı</h3>`
`<h4>Yazı</h4>`
`<h5>Yazı</h5>`
`<h6>Yazı</h6>`

---
## Input Tagı

İçerisine veri alan ve bu verileri işlemenizi sağlayan yazı kutularına (textbox) input denir. Inputlar type olmadan kullanılmaz. Tip olarak bir tip belirtmeli ve o formatta veri almalısınız. Aşağıda en yaygın kullanılan inputlar listelenmiştir.

`<input type="text" placeholder="metin giriniz">` - Düz bir biçimde yazı yazmanızı sağlayan textbox çıktısı sağlar.
`<input type="password" placeholder="şifre giriniz">`- Girdiğiniz tüm karakterleri • şeklinde gizleyerek gösteren textbox çıktısı sağlar
`<input type="email" placeholder="email giriniz">` - E-Mail formatı için kullanılan textbox. xxx@x.com gibi kullanılmazsa devam etmenizi engeller.
`<input type="number" placeholder="sayı giriniz">` - İçine yalnızca sayı girebilirsiniz. İçerisinde harf olarak yalnızca "e" çalışır. 
E'nin çalışma sebebi, sayıların toplam veya çarpım gibi sonuçlarında eğer büyük bir sayı çıktısı verilirse E olarak belirtilir.
`<input type="checkbox">` - Checkbox, yani seçim kutusu oluşturmanızı sağlayan input. 5 adet checkbox içerisinden 5'ini de seçebilirsiniz.

Örneğin, aşağıdaki çıktıda dilerseniz hepsini seçebilirsiniz. Dilerseniz yalnızca 1 adet.
`
<span> Hangi Şarkıcıyı Dinliyorsun?</span>
<input type="checkbox"> A 
<input type="checkbox"> B 
<input type="checkbox"> C 
`

`<input type="radio">` - Radio buton seçenekler arasından sadece bir adet seçmenizi sağlayan input tipidir. Örnek olarak, kayıt ol sayfasındaki cinsiyet seçimi radio button ile yapılabilir.

`<input type="submit" value="Gönder">` - Submit tipi, eğer bir form gönderiyorsanız, Formun işlemesi için gerekli buton tipidir. Verileri alır ve form içerisindeki yönergeleri uygulayarak işler.

`<input type="button" value="Tıkla">` - Düz butondur. a tagı verilerek link eklenebilir.

`<input type="reset" value="Sıfırla">`- Submit tipi butonun tam tersidir. POST etmek için doldurduğunuz verileri temizlemek için kullanılır ve FORM içerisindeki tüm inputları sıfırlar.

`<input type="file" name="myFile">` - Dosya yüklemek için kullanacağımız inputtur. Bu input, bizlerin bilgisayarımızdan dosya yüklemesine olanak sağlar.

`<input type="hidden" name="myHiddenValue">` - Hidden yani gizli input, bizlerin içerisinde verileri saklamamıza olanak sağlayan ve kullanıcıya gözükmeyen inputlardır.
Bu inputlarda genellikle kullanıcıların oturum kontrolleri bulunmaktadır.

`<input type="date" name="myDate">` - Bu input, bizlere dd,mm,yyyy şeklinde bir input verir. Gün, Ay, Tarih şeklinde seçim yapabilmemizi sağlar. Bu seçimleri dilerseniz yanındaki takvim butonuna basarak siz seçebilirsiniz.

`<input type="time" name="myTime">` - Time inputu date inputu ile aynı şekilde çalışmaktadır. Sadece, saat seçimi yapılmaktadır.

`<input type="range" name="myRange" min="0" max="100" value="50">` - Bazı E-Ticaret sitelerinde bulunan fiyat aralığını seç, özelliği kullandıran inputtur. Bu input ile sağa veya sola kaydırarak istediğiniz değerde durdurabilirsiniz. Bu kodta, 0-100 arasında bir değer seçmemiz istenmiş ve sayfa açıldığında ise bu değeri 50 olarak belirlemiş

`<input type="color" name="myColor" value="#ff0000">` - Bu input bizlere renk seçmemizi sağlayan renk paletini açar. Bu renk paleti ile bizler tüm renkleri seçebilir rgb, hex kodlarını görebiliriz.

`<input type="tel" placeholder="telefon numarası giriniz">` - Bu inputsa bizlere numara yazmamızı sağlar. Belirli formatın dışına çıktığınızda hata verecektir.

`<input type="url" placeholder="url giriniz">` - Bu input içine sadece URL adresi girmemizi kabul edecektir. Örn: https://google.com/ 

---
## BR ve HR Tagı

Bu tagların kullanımı aslında oldukça basittir. 

`<br>` - Satırlar arasında boşluk bırakmanızı sağlar

`<hr>` - Yatay çizgi eklemenizi sağlar. 

Örneğin: ______________________

---
 
## Div Tagı

Div, bir çok karışık elementi birleştirmek ve beraber bir düzene oturtmak amacıyla kullanılan tagdır. Class ile içine stil verebilirsiniz.

Örnek kullanım şekli aşağıdaki gibidir: 

`<div class="ornek"><input type="text" placeholder="İsim Giriniz"><input type="button" value="Butona Tıkla"></div>`


Not: Class değerini atadığınızda ya link tagı ile başka bir dosyadan ya da style tagı ile dosya içerisinden stil düzenlemesi yapabilirsiniz. Aşağıda stil ve link tagı kullanımı mevcut.

---

## style Tagı

Sayfa içerisindeki taglara stil vermek için kullanılan tag. Style tagı ile kullanım için div'de bir adet class'a sahip olmalısınız. 

Not: Style head tagı içerisinde veya body tagının başlangıcında bulunmalıdır.


Örnek bir style kodu:
`<style>.ornek{
background:#ff0000;
color: #fff;
width:300px;
height:150px;
</style>`

Örnek bir div kodu:
`<div class="ornek">Test Yazı</div>`

Bu kodun çıktısı, genişliği(width) 300, yüksekliği (height) 150 pixel, arkaplan rengi kırmızı ve içerisindeki "Test Yazı" adlı yazı beyazdır.


## Link Tagı

Link tagı, belirli stil (.css) dosyalarının .html dosyanızın içine entegre edilmesini sağlar.
Aşağıda basitçe örnek bir kullanımı vardır.
`<link rel="stylesheet" type="text/css" href="stildosyaniz.css">`


