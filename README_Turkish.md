# Yerçekimini kullanarak elektrik üretmek (G.E.G.)

- İngilizce seviyem iyi değil. Bu README.md dosyası çeviri yardımı ile ingilizceye dönüştürülmüştür.
- Orjinal döküman [README_Turkish.md](./README_Turkish.md) dosyasıdır.

## Önizleme

https://github.com/AhmetYildiz0/Generating-electricity-using-gravity/assets/76514989/e522691c-a4d8-4947-9345-540dff65f534

https://github.com/AhmetYildiz0/Generating-electricity-using-gravity/assets/76514989/35c3e52c-2e83-4c04-89bc-c9378251eedc

https://github.com/AhmetYildiz0/Generating-electricity-using-gravity/assets/76514989/c761d4f5-3066-476c-91c3-62d33293b9fc

## Parçalar
![Parçalar](./image_00002.png)


1. İp 
2. Sabit halat makarası	
3. Balon	
4. İçi su yada Tuzlu su dolu varil	
5. Boru
6. Hava vanası
7. Birbirine menteşe ile bağlı iki plaka
8. Hava pompasının balonu
9. Hava pompasının yayı
10. Kilit
11. Kilit yayı
12. Ağırlık sepeti 
13. Alüminyum profil
14. Yataklı rulman
15. Alüminyum çubuk
16. Birleştirici
17. Tek tönlü rulman
18. Koni dişli
19. Vites kutusu
20. Elektrik motoru
21. Hava girişi
		
## Çalışma prensibi
*	### Tek G.E.G
	1. Ağırlık sepeti, yerçekimi etkisiyle aşağı yönlü hareketini ip ile ara şafta aktarır. 
	2. Ara şaft, tek yönlü rulman ile sadece ağırlığın düşme hareketini ana şafta aktarır.  
	3. Ağırlık sepeti aşağı indikçe balon da suyun dibine iner. Suyun basıncı ile balonun içinde kalan hava da, hava pompasına akar.
	4. Ağırlık sepeti hava pompasına değmeden hemen önce hava vanası kapanır.
	5. Ağırlık sepeti, altındaki hava pompasını sıkıştırır ve tüm havayı, hava vanası kapalı olan boruya aktarır.
	6. Hava pompası tamamen sıkışıp kilitlendir. Hemen ardından hava vanası açılır.
	7. Borudaki tüm hava, boruya bağlı olan su yada tuzlu su dolu varilin içindeki balona aktarılır.
	8. İp ile ara şafta bağlı olan balon, suyun kaldırma kuvvetinin etkisiyle oluşan yukarı yönlü hareket ile ara şaftı döndürür.
	9. Dönen ara şaft, ağırlık sepetini tekrar yukarı kaldırır ve tek yönlü rulmanın bu hareketi ana şafta aktarmaz.
	10. Ağırlık istenen yüksekliğe geldiğinde hava pompasının kilidi açılır, yayın etkisiyle iç alanı artan pompa, balondaki havayı tekrar içine alır. 
	11. Suyun kaldırma kuvvetinden kurtulan ağırlık tekrar aşağı düşer ve tüm aşamalar baştan tekrarlanır.

*	### Çoklu G.E.G
	*	Karşılıklı iki G.E.G aynı ana şaftı paylaşabilir.
	*	Her bir G.E.G'in Ana şaftı birbirine eklenebilir.
	*	Elektrik üretiminin sabit devam edebilmesi için G.E.G'lerdeki ağırlıkların düşme zamanlamalarının ayarlanması gerekli.

*	### Elektrik Motoru Kısmı
	*	Ana şaft, sistemdeki düşen ağırlıkların toplamı kadarlık bir gücü vites kutusuna iletir.
	*	Elektrik motorunun tüm kapasitesini kullanmak için vites kutusu ana şaftın dönüşünü N katına çıkartır.
	*	Ve elektrik motoru elektrik üretir.
## Tasarım sırası
*	İhtiyaç duyulan elektrik miktarı belirlenir (kwh).
*	Elektriği üretmek için gereken elektrik motoru sayısı ve gücü belirlenir.
*	Elektrik motorlarının istenen gücü üretebilmesi için gereken motor devri sayısı belirlenir.
*	Belirlenen motor devri sayısına ulaşabilmeleri için gereken toplam güç miktarı kilograma dönüştürülür.
*	Belirlenen kilogram miktarı aşağıya düşen ağırlıkların toplamıdır. Bir bu kadar ağırlık da yukarı çıkan ağırlık miktarı olmalı bu yüzden toplam 2 ile çarpılır. 
*	Kaç tekli g.e.g. kullanılacağı belirlenir ve toplam ağırlık bu g.e.g.'lere paylaştırılır. Sistemin düzenli ve kesintisiz elektrik üretebilmesi için en az 3 g.e.g. olmalı.
*	g.e.g.'lerdeki hava pompasının ve balonun kaldırma gücü,  ağırlık sepetlerini kaldırabilecek kadar olmalı. 
*	g.e.g.'lerdeki diğer bütün parçaların ağırlığa ve balonun kaldırma gücüne dayanıklı olması gerekiyor.
*	Hava pompasının vanası ve kilidi, hem g.e.g.'lerin kendi döngüsü hem de g.e.g.'ler arasındaki döngünün sorunsuz devam edebilmesi için zamanlamaların ayarlanmasında kullanılır.
## Notlar
*	Görseller, G.E.G'in çalışma prensibini gösterebilmek için Unity(2022.3.11f1)'de hazırlanmış kaba animasyonlardır.
*	Başta merkezi elektrik üretim ve dağıtımının azalması için tasarladım.
*	Hala bir çok eksiği var. Bu tasarım G.E.G.'in final aşaması değil, tersine bebek adımıdır. Örneğin;
	*	Üretmek istenilen elektrik miktarına göre boyutları değiştirebilir, sayıları arttırabilir.
	*	Ana şafta dönemeçler eklenerek normalde art arda sıralanan g.e.g.'lerin alanı daha rahat bir şekilde yerleştirilmesi sağlanabilir.
	*	Destek kısmına ve ana şafta küçük değişiklikler ve eklemeler ile katlı bir tasarım oluşturulabilir. Böylece büyük çaplı elektrik üretimi için, yapımı ve taşıması maliyetli büyük parçalar kullanmak yerine küçük çok sayıda parça kullanılabilir.
	*	Su varili kapatılıp ağırlığın savrulması engellenirse, hareketli yerler de kullanılabilir.(Tırlar, Trenler, yük gemileri gibi)
*	Yeterli yapay yada doğal yer çekimi olan ve kaldırma kuvvetini oluşturabildiğiniz uzaydaki herhangi bir yerde kullanılabilir.
*	Mekanizmayı yapalidiğim kadar sadeleştirmeye çalıştım. Bu tasarımla amaçladığım; 
	*	rahatça üretilip kullanılabilmesi ,
	*	olabildiğince modüler olması,
	*	herhangi bir yere yada duruma, küçük bir kaç değişiklik ile uyum sağlaması,
	*	bozulduğunda kullanıcıların bile kolay bir şekilde tamir edebilmesi , 
	*	kullanılamaz hale geldiğinde çevreyi kirletmeden geri dönüştürülüp tekrar üretilebilmesi. Başka G.E.G'lerin ürettiği elektrik ile.
*	Ne yazık ki;
	*	Maddi sorunlar
	*	Teknik bilgi yetersizliği. (Hem öğrenip hem de yapmaya çalışırsam çok uzun sürecek.)
	*	Okul pek iyi gitmiyor. Okul dersleriyle ilgilenmem gerekiyor.(İskenderun Teknik Üniversitesi - Bilgisayar Mühendisliği - 4. sınıf sanırım)
*	Yukarıdaki başlıca sebeplerden ve başka küçük sorunlardan dolayı bir G.E.G. üretemedim. Gerçek dünyada ne kadar verimli çalıştığını bilmiyorum.
*	Ama eminim ki açık kaynak topluluğu, üniversiteler, firmalar ve ülkeler, G.E.G.'i dünyanın yeni, en temiz ve en verimli enerji kaynağı haline getireceklerdir.
## Telif
Bu tasarımı ve fikri özgürce üretebilir, kullanabilir, geliştirebilir ve satabilirsiniz. Bir teşekkür etseniz yeter.
