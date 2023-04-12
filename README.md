<div align="center">
<img src="https://user-images.githubusercontent.com/33163650/231457894-7e2a11c1-3334-49f0-b538-a0519ecd91bd.jpg" width="250" height="200">
</div>


<h1 align="center">Python'da Türkçe Eş Anlamlı Kelime Değişimi </h1>
<p align="justify">

Türkçe doğal dil işleme kütüphaneleri genellikle İngilizce dili için geliştirilmiş olan kütüphanelerin Türkçe versiyonlarıdır. Ancak, Türkçenin dil yapısı İngilizce ile farklılık gösterdiği için bu kütüphaneler bazı sorunlar yaşayabilir. Bu nedenle, Türkçe doğal dil işleme uygulamalarında eş anlamlı kelimelerin belirlenmesi zor olabilir. Buna çözüm olarak araştırmalar yaptım ve <b>Yusuf Ustanın github eş anlamlı kelimeler reposunu buldum.</b> (json, csv, xml <a href="www.github.com"> <b> REPOYU GÖRMEK İÇİN TIKLAYINIZ </b></a>) Bu repoyu Pythona uyarlayıp Eş anlamlı kelime girince, sonucunda eş anlamını bulan kodu yazdım.</p>

*  [:fire: Geliştirici](#fire-geliştirici)
*  [:hash: Kod Nasıl Çalışır?](#hash-kod-nasıl-çalışır)

# :fire: Geliştirici
| Adı Soyadı | 
| :--- | 
| [Burak ÖZDEMİRTAŞ](https://github.com/burakozdemirtas) |


# :hash: Kod Nasıl Çalışır?
<p align="justify">
Bu kod, eş anlamlı kelimelerin bulunduğu bir CSV dosyasını okuyarak, belirli bir metindeki kelimelerin eş anlamlılarını değiştirmek için kullanılır.

İlk olarak, pandas kütüphanesi kullanılarak 'esanlamlilar.csv' dosyası okunur ve veriler bir pandas DataFrame nesnesine yüklenir. Ardından, synonyms_dict adlı boş bir sözlük oluşturulur.

Daha sonra, df DataFrame'inin her satırında döngü oluşturularak, kelime ve eş anlamlıları alınarak synonyms_dict sözlüğüne eklenir.

Daha sonra, 'message' adlı bir metin değişkeni tanımlanır ve split() fonksiyonu kullanılarak kelimelere ayrılır. Bu kelimelerin her biri için, eğer kelime sözlükte varsa, ilk eş anlamlı kelime seçilir ve orijinal kelime yerine geçirilir.

En son olarak, yeni kelime listesi 'new_message' oluşturulur ve bu kelime listesi boşluk karakteriyle birleştirilerek, eş anlamlıları değiştirilmiş metin oluşturulur ve print() fonksiyonu kullanılarak ekrana yazdırılır.  </p>
