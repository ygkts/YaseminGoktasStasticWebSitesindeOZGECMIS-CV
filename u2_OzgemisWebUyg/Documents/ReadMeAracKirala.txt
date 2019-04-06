	KULLANILAN TEKNOLOJ�LER:

	- Microsoft Sql Server 2014
	- Visual Studio Enterprise 2015
	- Entity Framework
	- c# Programlama Dili
	- .net Framework

	PROGRAMIN AMACI :

	- Bu program, bir ara� kiralama �irketinde �al��anlar�n internetsiz bir ortamda gerekli t�m i�lemleri yapabilmesi i�in yaz�lm��t�r.

	PROGRAMIN KULLANIM A�AMALARI:

	Program �al��t�r�ld���nda ilk olarak KULLANICI G�R��� ekran� kar��m�za ��kar. Burada bu formun formLoad eventinde otomatik olarak email ve �ifre atanm��t�r. Bu haz�r gelen bilgiler ile giri� yap�labilinece�i gibi kullan�c�lar veri taban�ndaki di�er kullan�c�lar�n bilgileriyle de giri� yap�labilir. �ki textbox da dolu ise enter tu�una basarak anasayfa formuna giri� yapabilirsiniz.
	
	�lk olarak anasayfan�n sa� �st k��esinde giri� yapan kullan�c�n�n ad� ve soyad� bilgisi belirmektedir. ��k�� yap butonu ile formun kapanmas�n� sa�lay�p programdan ��kabilirsiniz. 
	
	Men� Strip'in ilk men�s� M��teri ��lemleri men�s�d�r. Burada m��teri ekleme, ��karma ve bilgilerini g�ncelleme i�lemleri yap�labilir. Bu men�ye t�klad���m�zda AnasayfaFormunun i�ine M��teri��lemleri formunu alm�� oluruz. A��lan bu form m��teri i�in her t�rl� ihtiya� duyulan bilgileri i�ermektedir. PictureBox'a bir m��teri resmi ekleyerek bu resmi de veri taban�na ekleyebilirsiniz. Bu, pictureBox'taki resmin Byte [] t�r�ne yani bir byte dizisine �evirilmesiyle ger�ekle�tirilmi�tir. Resim haricindeki bilgiler de textboxlar, comboboxlar, datetimepicker'lar kullan�larak al�nm��t�r. Bu alanda datagridbiew �zerinde bir sat�ra t�kland���nda t�m bilgiler ayr� ayr� g�ncelleme yapabilmek i�in yerlerine yerle�tirilir. Bu i�lem datagridview'in cellmouseclick event'ine yaz�lm��t�r.
	
	Sonraki men� Ara� ��lemleri men�s�d�r ve bize Ara� ��lemleri Formunu a�ar. Bu formda m��teri i�lemlerindeki gibi eklem, ��karma ve g�ncellem i�lemlerini veirt taban�m�za yapabilmektir. E�er �irket yeni bir ara� ald�ysa veya ara� bilgisi hakk�nda g�ncellem yapacak ise veya ar�zal� ya da �ok eski bir arac� sistemden ��karmak istiyorsa bu forma ihtiya� duymaktad�r.
	
	Di�er men� Kira ��lemleri ad�ndad�r. Buraya t�kland���nda 
 adet alt men� kar��m�za ��kar: Ara� Kirala ve Kiradan Ara� Al . Bu iki men� de ayn� formu a�maktad�r. Farkl� bir kullan�m olmas� a��s�ndan burada ayr� ayr� formlar olu�turmak yerine ayn� tablo�zerinde i�lem yap�laca�� i�in tek formun iki alt men� i�in de gerekli yerleri aktif b�rak�larak kullan��l� bir form olu�turulmu�tur. Bu form da Ara� Kirala ile Kiralam�� ara�lar tablosuna ekleme ve g�ncelleme i�lemi yap�l�r ve bu kiralama yap�ld���nda M�saiit Ara�lar tablosundan o plakal� ara� silinmi�tir. Kiradan Ara� Al alt men�s� ise Kiralanm�� Ara�lar tablosundan silme i�lemi yapar. BU silme ger�ekleti�inde bu ara� ms�ait ara�lar tablosuna tekrar eklenmi� olur.
	
	Raporlar men�s� kiralanm�� bir ara� tesllim al�nd�ktan sonra e�er b�y�k bir hasar� oldu�u anla��l�rsa o ara� hakk�nda kiralayan ki�iye hasar �cretini alabilmek i�in rapor tutulur.  Rapor tutalan ara� M�sait Ara�lar k�sm�ndan (tablosundan) ��kar�lm��t�r. E�er bu raporlar tablosundaki ara� da silinir ise Ara�lar tablosundan da bu ara� silinmektedir. ��nk� art�k o ara� �irket prensipleri gere�i �irketin galerisinde tutulmak ve bir m��teriye kiralanmak istenmez.
	
	Hakk�nda men�s� ile otomasyon kullan�c�s�na, otomasyonu tan�tmak amac� ile k�saca bilgilendirme yap�lm��t�r. Neyin ne i�e yarad��� neyi nas�l kullanaca�� hakk�nda bilgiler bu form sayesinde kullan�c�ya iletilir.
	
	Ayarlar men�s� sisteme giri� yapan otomasyon kullan�c�s�n�n yetki d�zeyi 5 ve �zeri ise eri�ilebilmektedir. E�er bu alt men�y� a�abilme yetkiniz var ise bu k�s�m kullan�c�� ekleme silme veya bilgileri g�ncellemeye yaramaktad�r. Yetki d�zeyi kullan�c�lar tablosunda YetkiD�zeyi alan�nda tutulur ve buradan �ekilerek program kodu i�inde kontrol ger�ekle�tirilir.