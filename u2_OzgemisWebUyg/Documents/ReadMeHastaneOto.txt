	KULLANILAN TEKNOLOJ�LER:

	- Microsoft Sql Server 2014
	- Visual Studio Enterprise 2015
	- Entity Framework
	- c# Programlama Dili
	- .net Framework

	PROGRAMIN AMACI :

	- Bu program, hastanede �al��an memurlar�n internetsiz bir ortamda gerekli t�m hasta, doktor, randevu i�lemleri yapabilmesi i�in yaz�lm��t�r.

	PROGRAMIN KULLANIM A�AMALARI:
	
	�lk olarak DB klas�r� alt�ndaki HastaneTakipOtomasyonYG.bak backup dosyas�n� veritaban�n�za aktarmal�s�n�z. Daha sonra progrma� �al��t�r�n�z.

	Program �al��t�r�ld���nda ilk olarak KULLANICI G�R��� ekran� kar��m�za ��kar. Burada bu formun formLoad eventinde otomatik olarak email ve �ifre atanm��t�r. Bu haz�r gelen bilgiler ile giri� yap�labilinece�i gibi kullan�c�lar veri taban�ndaki di�er kullan�c�lar�n bilgileriyle de giri� yap�labilir. �ki textbox da dolu ise enter tu�una basarak anasayfa formuna giri� yapabilirsiniz.	
	
	Ayarlar men�s� sisteme giri� yapan otomasyon kullan�c�s�n�n yetki d�zeyi 5 ve �zeri ise eri�ilebilmektedir. E�er bu alt men�y� a�abilme yetkiniz var ise bu k�s�m kullan�c�(memur) ekleme silme veya bilgileri g�ncellemeye yaramaktad�r. Yetki d�zeyi kullan�c�lar tablosunda YetkiD�zeyi alan�nda tutulur ve buradan �ekilerek program kodu i�inde kontrol ger�ekle�tirilir. Haz�r olarak gelen ak@gmail.com adresinin yetki d�zeyi bu ayarlara girebilmek i�in yeterlidir.

	Ba�ar�l� bir �ekilde girii� yap�ld�ktan sonra kar��m�za anasayfa ��kar. Burada menustrip ile bir�ok i�leme ula�abiliriz. Sa� �st k��ede 3 adet picturebox bulunmaktad�r. �zerlerine t�klad�n��nda geli�tiricinin ( YASEM�N G�KTA� ) kullan�c� belirtilen web adreslerine y�nlenmi� olur.

	Ekle/ G�ncelle/ Sil ��lemleri MenuStrip'inde Hasta, Doktor, Hem�ire, B�l�m veri tabanlar�na CRUD i�lemleri uygulanmak amac�yla haz�rlanm�� formlar bulunur. Hasta ve Doktor'un profill resimleri eklenmi�tir fakat Hasta randevu al�rken ger�ek hayatta sisteme bir foto�raf y�klemeyece�i i�in Hasta formunda resim i�lemleri kullan�lmamas� tercih edilmi�tir. Di�er CRUD i�lemleri her form i�in ge�erlidir.

	Randevu formunda da CRUD i�lemleri mevuttur. Burada ek olarak Comboboxlar�n textchange eventleri ile birbirleri aras�nda ba�lant� vard�r. Ayr�ca �devde istenen se�ilen doktor ad�na g�re tabloda b�l�m ad�n�n otomatik olarak gelmesi i�lemi de ba�ar�l� bir �ekilde linq komutlar� kullanarak ger�ekle�tirilmi�tir. Detayl� bilgi i�in kodlar� inceleyebilirsiniz. Kod i�inde yorum sat�r� olarak bir ka� a��klama daha mevcuttur. Burada randevu tarihi se�ilebilece�i gibi saati de se�ilmektedir. Saat kontrol� i�in ayr� bir tablo olu�turulmu� ve Durum ismindeki bir kolonda saattlerin m�sait olma durumlar� 1 ve 0 ile ifade edilmi�tir. bu 1 ve 0 de�erleri formda yap�lan i�leme g�re dinamik olarak g�ncelenmektedir. Bu randevu saati combobox'�n� dolduran metod2daki linq komuttu ile ger�ekle�mi�tir. Detayl� bilgi i�in kodlar� inceleyebilirsiniz.