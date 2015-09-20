---
layout: post
language: tr
title: "Yapısal Gazetecilik ve Ağ Haritalama Hackathonu Dökümantasyonu"
subtitle: "12-13 Eylül 2015 İstanbul Hackathonu"
author:     "Graph Commons"
header-img: "img/istanbul-2015/Graphcommons-hackathon-2015-Istanbul-photo.jpg"
description: "Yapısal Gazetecilik ve Ağ Haritalama Hackathon'u Dökümantasyonu, 12-13 Eylül, 2015"
---

[Click here for English](/hackathons/2015/08/21/istanbul-yapisal-gazetecilik-documentation-en/)

[Graph Commons](https://graphcommons.com) tarafından düzenlenen [2 günlük hackathon](https://graphcommons.github.io/hackathons/2015/08/21/istanbul-yapisal-gazetecilik/) TMMOB Mimarlar Odası İstanbul Karaköy'deki mekanında gerçekleşti. Katılımcılar insan hakları, sivil toplum, ve hak gazeteciliği alanlarında kritik konulara dair verileri modellediler ve çeşitli kaynaklardan yığın veri toplayıp ilişki haritaları çıkaran bilgisayar uygulamaları geliştirdiler.

Aşağıda hackathonda geliştirilen araçlar, linkler, interaktif haritalar, fotoğraflar ve ekran görüntülerini kısa açıklamalarla toparladık.

# Geliştirilen Araçlar
Mentörlerle beyin fırtınası sonucu ortaya çıkan modellere göre programatik veri derleyen ve [Graph Commons API](https://graphcommons.com/dev) kullanarak harita yaratan uygulamalar geliştirildi.

Github üzerinde ulaşılabilen bu açık kaynaklı araçlara katkı yapmak isterseniz doğrudan kod deposundan iletişime geçiniz.

### Graph-Commons-Excel-Lab
[Graph-Commons-Excel-Lab](https://github.com/Batierk/Graph-Commons-Excel-Lab) – Minimal bir arayüz ile Excel tablosundan ağ haritası oluşturmayı sağlar. Excel dosyanızı yükledikten sonra 2 sütun seçip arasındaki ilişkiyi tanımlıyorsunuz ve uygulama sizin için haritayı yaratıyor. İstenildiği kadar iki kolon arası ilişki tanımlanabiliyor. C#, ASP, ve Javascript ile [Batı Erk Yılmaz](https://graphcommons.com/users/1c1cf322-9514-495b-b080-128fcec357e7) tarafından geliştirildi.

### Graph Commons Twitter Entegrasyonu
[graphcommons-egt](https://github.com/mehmetatas/graphcommons-egt) – Bir hashtag seçtiğinizde, bunu içeren tweetleri ve hesapları toplar, Neo4j ve Graph Commons'a import eder. Javascript Node.js ile [Mehmet Ataş](https://graphcommons.com/users/60f7f782-f56a-488d-b223-61621ddc1c2c) tarafından geliştirildi.

### TBMM Scraper
[TBMM scraper](https://github.com/meclistakip/tbmm-scraper) – Milletvekili biyografileri, komisyonlar, kanun teklifleri, ve partileri dönemlerine göre verileri TBMM'den çeker ve ilişkilendirerek bir "bürokrasi ağ haritası" yaratır. Node.js ile [Ahmet Kızılay](https://graphcommons.com/ahmetkizilay) tarafından ve [Ufuk Kayserilioglu](https://graphcommons.com/users/542a548f-104f-4f35-9275-a297fbf5c122) katkılarıyla geliştirildi.

### Graph Commons TBMM Önergematik
[Önerge Crawler](https://github.com/krk/onerge-crawler) – [tbmm.gov.tr](https://www.tbmm.gov.tr/) adresinden Soru Önergeleri çeker, ilişkili milletvekillerini ve partileri bağlayarak ağ haritası oluşturur. C# ile  [Kerem](https://graphcommons.com/users/e7bda695-c8c6-47da-85ec-57962639a08b) tarafından geliştirildi.


# Geliştirilen Ağ Haritaları

Hackathon'da programatik ya da manuel olarak derlenen verilerden interaktif ağ haritaları yaratıldı. Yapılan haritalar okumaya ve analize tabi tutuldu, tartışıldı ve Graph Commons üzerinde yayınlandı.

### Mega İstanbul Ağ Haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/Mega-Projeler-Tabanlioglu-Arolat-Mimarlik.png">
[Mega İstanbul Ağ Haritası](https://graphcommons.com/graphs/24d0e29b-8c98-4842-80a5-b2dcfd84bf5a) 103 İnşaat, 92 Proje, 88 Mimar, 90 Müteahhit ve aralarında ilişkilerden oluşan harita megaprojeleristanbul.com verisiyle geliştirildi. Proje boyutları yatırım miktarına göre gösterilmekte. Harita [Yakup Çetinkaya](https://graphcommons.com/users/f6bf26e7-f75e-43d9-bdd6-11f869e4c2ed) tarafından geliştirildi.

### Türkiye İşçi Eylemleri Haritası, Ocak 2015
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/turkiye-isci-eylemleri-ag-haritasi-ocak-2015.png">
[Türkiye İşçi Eylemleri Haritası](https://graphcommons.com/graphs/00af1cd8-5a67-40b1-86e5-32beae436f7c) Direniş İzleme Grubu'nun derlemekte olduğu veriler kullanılarak 2015 Ocak ayı için yapıldı. Harita 35 Sendika, 97 İşyeri, 10 İstihdam türü, 32 Şehir, 17 Eylem, 7 Eylem türü, ve 27 Sektör içermekte. Harita [Batı Erk Yılmaz](https://graphcommons.com/users/1c1cf322-9514-495b-b080-128fcec357e7) tarafından üretildi.

###  Twitter'da #EGT hashtag ilişki haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/twitter-egitim-reformu-EGT-hashtag-iliski-haritasi.png">
[#EGT hashtag ilişki haritası](https://graphcommons.com/graphs/5cb7ba29-79b2-42d4-94b0-e8597871bf5b) Twitter'da eğitim reformu için kullanılan hashtag ile beraber kullanılan diğer hashtagler ve hesapları arası ilişkileri gösterir. 324 Hesap, 33 Tag, 29 Tweet ve aralarında Tweet edilme, taglenme, retweet edilme ilişkilerini barındırır. Harita [Mehmet Ataş](https://graphcommons.com/users/60f7f782-f56a-488d-b223-61621ddc1c2c) tarafından geliştirildi.

### Kadın Cinayetleri 2010: Fail-öne sürülen sebep örüntüsü
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/Kadin-Cinayetleri-2010-fail-onersurulen-sebep-agi.png">
[Kadın Cinayetleri 2010 ilişki haritası](https://graphcommons.com/graphs/43a7a148-cf2e-40d7-8d9a-3f29c2d9b16a) 38 Sebep ve 18 Fail ve aralarındaki ilişkileri gösterir. Bianet'ten alınan verilerle harita [Sevil Seten](https://graphcommons.com/users/0a426059-a35e-40dd-b533-96e43a36d70c) tarafından geliştirildi.

### Anıt Sayaç Ağ Haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/AnitSayac-kadin-cinayetleri.png">
[Anıt Sayaç Ağ Haritası](https://graphcommons.com/graphs/337a0a01-0a51-4e7f-a761-5475ae9524e3?auto=true&layout=fa2), Kadın cinayetlerinin kategorik analizi. Anıt Sayaç, Türkiye’de kadına yönelik şiddetten ölen kadınların anısını yaşatmak için internet üzerinden kurulmuş bir anıt ve her gün güncellenen bir sayaçtır. [anitsayac.com](http://anitsayac.com/) verisiyle yapılan ağ haritası 1330 cinayet vakasını tarar ve 99 Fail, 46 Yöntem, 132 Sebep içerir. Harita [Yakup Çetinkaya](https://graphcommons.com/users/f6bf26e7-f75e-43d9-bdd6-11f869e4c2ed) tarafından geliştirildi.

### Şeylerin İnterneti (IoT) Sektör Haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/internet-of-things-categories-startups-cities-network-map.png">
[Şeylerin İnterneti (IoT) Sektör Haritası](https://graphcommons.com/graphs/50af620a-5b9f-4bc5-9b15-018c4626b645) IoT ürünü geliştiren 100 Şirket, 39 Şehir, 10 Sektör ve ilişkilerini içerir. Angel.co sitesinden çekilen verilerle oluşturulan harita [Asli Yazagan](https://graphcommons.com/users/7fda641f-3515-4581-8e1e-82d85c013c87) tarafından geliştirildi.

### İnternet Yasakları ve Karar Mercileri Haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/turkiye-internet-yasaklari-sansur-karar-merci-haritasi.png">
[İnternet Yasakları ve Karar Mercileri Haritası](https://graphcommons.com/graphs/0a86d5a8-f80e-4d11-b39c-d6ba7b6657d3?show=Graph&auto=true) Türkiye'de sansürlenmiş 1061 Websitesi ve 161 Mahkeme ve aralarında mahkeme emri ilişkisi içerir. engelliweb.com adresinden yeralan veriler sansürün boyutunu yeterince yansıtmasa da ender kaynaklardan olduğu için kullanılmıştır. Site kapatmalarına yol açan savcılar ve hakimlere dair bilgiler çok kritiktir ancak maalesef bulunamamaktadır. Harita [Ceyhun Enki Aksan](https://graphcommons.com/users/85dbf926-cd78-4dbc-bf4e-a005b7c26d38) ve [Raldu](https://graphcommons.com/users/bb372a3b-72ae-4040-be5c-a44c83809043) tarafından geliştirildi.

### TBMM 25. Dönem Soru Önergeleri Konu ve Milletvekili Ağı
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/TBMM-25-Donem-Soru-onergeleri-Konu-Milletvekili-agi.png">
[Soru Önergeleri konu vekil ağı](https://graphcommons.com/graphs/482c0a5f-45ca-48ae-b0bc-f49be66fe95d?auto=true) 25inci dönem için hangi partiden hangi vekilin hangi konularda soru önergesi verdiğini gösteren bir haritadır. Veri derleme ve haritalama [Ufuk Kayserilioglu](https://graphcommons.com/users/542a548f-104f-4f35-9275-a297fbf5c122) tarafından yapıldı.

### TBMM Soru Önergeleri Bakanlıklar Vekiller Ağı
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/TBMM-Soru-onergeleri-Bakanliklar-Milletvekili-agi.png">
[Soru Önergeleri Bakanlıklar Vekiller Ağı](https://graphcommons.com/graphs/37eb6a2d-26e4-4c79-9d71-75761458fd2f?auto=true&layout=fa2) TBMM'den alınan verilere göre 33 Bakanlık, 4 Parti, 1211 Soru Önergesi, 189 Milletvekili ve aralarındaki "muhatap", "sahiplik", "üyelik" ilişkilerini içerir. Veri derleme ve haritalama [Kerem](https://graphcommons.com/users/e7bda695-c8c6-47da-85ec-57962639a08b) tarafından yapıldı.

### 2013 Sonrası İşinden olan Gazeteciler Haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/2013-Sonrasi-Medya-calisanlarinin-kovulmalari-yeni-isleri.png">
[2013 Sonrası İşinden olan Gazeteciler Haritası](https://graphcommons.com/graphs/fd7b810b-be69-4fd9-838a-1ab9b67bd7bf) medya çalışanlarının kovulmaları, sebepleri ve yeni işlere geçişlerini gösterir. 40 Gazeteci, 15 Gazete, ve 2 Sebep içerir. Haritadan gazetecilerin eski işlerinden yeni işlere geçişleri takip edilebilir. Veri derleme ve haritalama [Mohan Ravichandran](https://graphcommons.com/users/656e50bd-1a46-4b81-b892-f85704b9c17c), [Kerem Başkaya](https://graphcommons.com/users/2a0b6ef6-cc7d-4e24-b182-ffcd818b5cf3), [Osman Başkaya](https://graphcommons.com/users/93a01de5-a445-400d-8a1a-9e485cbd3fc8) tarafından yapıldı.


### 23. ve 25. Dönem Milletvekili Olan Gazeteciler Haritası
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/23.donem-Milletvekili-Olan-Gazeteciler-Haritasi.png">
[23. Dönem Milletvekili Olan Gazeteciler Haritası](https://graphcommons.com/graphs/7990bec9-d50b-4765-baf8-3421ae5b17bd)
<img src="https://graphcommons.github.io/hackathons/img/istanbul-2015/25.donem-Milletvekili-Olan-Gazeteciler-Haritasi.png">
[25. Dönem Milletvekili Olan Gazeteciler Haritası](https://graphcommons.com/graphs/3426266e-32cc-42d7-a0c7-32f943a61a5f)

23üncü ve 25inci dönemlerde hangi gazeteciler hangi partiden milletvekili oldu? Veri derleme ve haritalama [Atınç Gürçay](https://graphcommons.com/users/fc10d290-0cc4-4cf2-96ec-b524e885682f), [Sidar Bayram](https://graphcommons.com/users/591b6a83-b592-40c0-b94b-f1caaf197d40), [Dygu](https://graphcommons.com/users/61f56937-3f8d-4756-bf6a-838d5f80c51d) tarafından yapıldı.

---

Hackathon'da yapılan işlerle ilgili sorunuz ya da yorumlarınız için doğrudan yapan kişilerle iletişime geçiniz. Hackathon hakkında genel sorular ve yorumlar için bize [Graph Commons iletişim sayfası](https://graphcommons.com/contact) üzerinden ulaşabilirsiniz.

_Bu Hackathon [Ayça Aldatmaz](https://twitter.com/manythingoes) ve [Ahmet Kızılay](https://twitter.com/ahmetkizilay)'ın emeği ve katılan tüm [mentörlerin](https://graphcommons.github.io/hackathons/2015/08/21/istanbul-yapisal-gazetecilik/#konular-mentorler-kaynaklar) desteği olmadan gerçekleşemezdi. Kendilerine çok teşekkür ediyoruz. Ayrıca duyurunun yayılmasında yardımcı olan [Serdar Paktin](https://twitter.com/paktin)'a da tekrar teşekkürler._

_[Fotoğraf](https://twitter.com/gulayozkan/status/643096200271556608) için [Gülay Özkan](https://twitter.com/gulayozkan)'a teşekkürler._
