<div align="center">
<img src="https://user-images.githubusercontent.com/33163650/231457894-7e2a11c1-3334-49f0-b538-a0519ecd91bd.jpg" width="250" height="200">
</div>


<h1 align="center">Python'da Türkçe Eş Anlamlı Kelime Değişimi/Python Turkish Synonym Replacement </h1>
<p align="justify">

Türkçe doğal dil işleme kütüphaneleri genellikle İngilizce dili için geliştirilmiş olan kütüphanelerin Türkçe versiyonlarıdır. Ancak, Türkçenin dil yapısı İngilizce ile farklılık gösterdiği için bu kütüphaneler bazı sorunlar yaşayabilir. Bu nedenle, Türkçe doğal dil işleme uygulamalarında eş anlamlı kelimelerin belirlenmesi zor olabilir. Buna çözüm olarak araştırmalar yaptım ve <b>Yusuf Ustanın github eş anlamlı kelimeler reposunu buldum.</b> (json, csv, xml <a href="https://github.com/yusufusta/Es-Anlamlilar"> <b> REPOYU GÖRMEK İÇİN TIKLAYINIZ </b></a>) Bu repoyu Pythona uyarlayıp Eş anlamlı kelime girince, sonucunda eş anlamını bulan kodu yazdım.</p>

Natural language processing libraries for Turkish are generally the Turkish versions of libraries developed for the English language. However, since the structure of the Turkish language is different from English, these libraries may encounter some problems. Therefore, identifying synonyms in Turkish natural language processing applications can be challenging. As a solution, I conducted research and found <b>Yusuf Usta's GitHub repository for synonyms.</b> (json, csv, xml <a href="https://github.com/yusufusta/Es-Anlamlilar"> <b>CLICK HERE TO VIEW THE REPO</b></a>) I adapted this repository to Python and wrote a code that finds the synonym when an synonymous word is entered.

*  [:fire: Geliştirici/Developer](#fire-geliştirici-developer)
*  [:hash: Kod Nasıl Çalışır?/How does the code work?](#hash-kod-nasıl-çalışır-how-does-the-code-work)

# :fire: Geliştirici / Developer
| Adı Soyadı / Name Surname | 
| :--- | 
| [Burak ÖZDEMİRTAŞ](https://github.com/burakozdemirtas) |


# :hash: Kod Nasıl Çalışır? How does the code work?
<p align="justify">
Bu kod, eş anlamlı kelimelerin bulunduğu bir CSV dosyasını okuyarak, belirli bir metindeki kelimelerin eş anlamlılarını değiştirmek için kullanılır.

İlk olarak, pandas kütüphanesi kullanılarak 'esanlamlilar.csv' dosyası okunur ve veriler bir pandas DataFrame nesnesine yüklenir. Ardından, synonyms_dict adlı boş bir sözlük oluşturulur.

Daha sonra, df DataFrame'inin her satırında döngü oluşturularak, kelime ve eş anlamlıları alınarak synonyms_dict sözlüğüne eklenir.

Daha sonra, 'message' adlı bir metin değişkeni tanımlanır ve split() fonksiyonu kullanılarak kelimelere ayrılır. Bu kelimelerin her biri için, eğer kelime sözlükte varsa, ilk eş anlamlı kelime seçilir ve orijinal kelime yerine geçirilir.

En son olarak, yeni kelime listesi 'new_message' oluşturulur ve bu kelime listesi boşluk karakteriyle birleştirilerek, eş anlamlıları değiştirilmiş metin oluşturulur ve print() fonksiyonu kullanılarak ekrana yazdırılır. 
 
</br>
This code is used to replace the synonyms of certain words in a given text by reading a CSV file that contains synonym words.

First, the 'esanlamlilar.csv' file is read using the pandas library and the data is loaded into a pandas DataFrame object. Then, an empty dictionary called synonyms_dict is created.

Next, a loop is created to iterate through each row of the df DataFrame, and the word and its synonyms are extracted and added to the synonyms_dict dictionary.

Then, a text variable called 'message' is defined and split() function is used to split it into words. For each of these words, if the word exists in the dictionary, the first synonym word is selected and replaces the original word.

Finally, a new word list 'new_message' is created and this list is joined with a space character to create the final text with replaced synonyms. The print() function is used to display the modified text on the screen.
</p>



