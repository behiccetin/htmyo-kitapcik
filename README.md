# Kitapçık Oluşturucu

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24226187.svg)](https://doi.org/10.5281/zenodo.24226187)

**Burdur Mehmet Akif Ersoy Üniversitesi, Bucak Hikmet Tolunay Ulaştırma ve Lojistik Meslek Yüksekokulu**

Yüksekokulun Sınav Soruları Formu (PFRM-217), kendi Word dosyanız ya da bir metin dosyasıyla (.txt, Aiken biçimi dahil) hazırladığınız A kitapçığından, soruların ve şıkların yeri değiştirilmiş **B, C, D ve E kitapçıklarını** ve her birinin **cevap anahtarını** üreten, tek dosyalık web aracı. Aynı araç sınavın **ölçme planını** hazırlar ve sınavdan sonra madde analiziyle birlikte aynı düzende **ölçme sonuçlarını** verir.

**Kullanmak için:** https://behiccetin.github.io/htmyo-kitapcik/

**Önceki sürümler:** https://behiccetin.github.io/htmyo-kitapcik/surumler/ (sayfanın altındaki sürüm numarasına tıklayınca da açılır; eski bir sürümle hazırlanmış kitapçıklar aynı üretim koduyla yeniden üretilebilir)

**Resimli yardım:** https://behiccetin.github.io/htmyo-kitapcik/yardim.html (ekran görüntüleriyle adım adım anlatım ve deneme dosyaları)

Sistem mimarı ve geliştirici: **Öğr. Gör. Dr. Behiç ÇETİN**
Burdur Mehmet Akif Ersoy Üniversitesi, Bucak Hikmet Tolunay Ulaştırma ve Lojistik Meslek Yüksekokulu

## Nasıl kullanılır?

Yalnızca A kitapçığını hazırlarsınız; B, C, D ve E kitapçıkları ondan türetilir.

### A. Yüksekokulun şablonuyla (Sınav Soruları Formu, PFRM-217)

1. Yüksekokulun web sitesindeki [Personel Formları](https://htmyo.mehmetakif.edu.tr/content/19994) sayfasından *Sınav Soruları Formu (Test)* ya da *(Klasik ve Karma)* şablonunu indirin.
2. Ders ve sınav bilgilerini doldurun, soruları ve şıkları ilgili kutulara yapıştırın.
3. Kullanmadığınız "Ek soru tipleri" örneklerini ve boş kalan soruları silip dosyayı kaydedin.
4. Dosyayı araca yükleyin, doğru cevapları işaretleyin, kitapçıkları seçin ve **Kitapçıkları oluştur**'a basın.
5. İnen dosyaları Word'de açıp kontrol edin. Kitapçık türü alanı her dosyada kendi harfiyle doludur.

### B. Kendi Word dosyanızla

- Her soru yeni bir paragrafta ve `1.` ya da `1)` ile başlamalı (Word'ün otomatik numaralandırması da olur).
- Her şık **ayrı satırda** ve `A)`, `B)` (ya da `a)`, `A.`) ile başlamalı.
- Görsel, tablo veya öncüller soru ile şıklar arasında olabilir; soruyla birlikte taşınır.
- Şıklar aynı satıra yan yana yazılmışsa soru yer değiştirir ama şıkları karıştırılamaz.
- Sorulardan önceki başlık ve öğrenci bilgileri ile son sorudan sonraki yazılar yerinde kalır.
- Her kitapçığın en üstüne sağa yaslı "Kitapçık Türü: B" satırı eklenir.
- **Bir şıkkın içinde Enter'a basmayın.** Uzun şık kendiliğinden alt satıra kayar; Enter'a basılırsa şık ikiye bölünür ve araç o sorunun şıklarını karıştırmaz.
- Ortak metne bağlı sorularda metnin başına `7-9. soruları aşağıdaki metne göre cevaplayınız.` gibi bir satır yazın; sorular metinle birlikte taşınır, başlıktaki numaralar her kitapçıkta düzeltilir.

```
1. Aşağıdakilerden hangisi bir taşıma türüdür?
A) Depolama
B) Karayolu
C) Paketleme
D) Etiketleme
E) Sayım
```

### C. Metin dosyasıyla (.txt ya da Aiken)

Sorular arasında bir boş satır bırakın, şıkları `A)` ya da `A.` ile başlatın. Aiken biçiminde şıklardan sonra `ANSWER: B` (ya da `CEVAP: B`) satırı gelir ve cevaplar kendiliğinden işaretlenir. Araç metinden düzenli bir A kitapçığı (Word) oluşturur.

```
Aşağıdakilerden hangisi bir taşıma türüdür?
A) Depolama
B) Karayolu
C) Paketleme
D) Etiketleme
E) Sayım
ANSWER: B
```

Aracın "Nasıl kullanılır?" bölümünden örnek Aiken ve düz metin dosyaları indirilebilir.

## Çalışmayı kaydetme (.htmyo)

Araç hiçbir şeyi kendisi saklamaz. Sayfanın üstündeki **Çalışmayı kaydet (.htmyo)** düğmesi o ana kadar yapılan her şeyi (A kitapçığı dosyası, cevaplar, ÖÇ'ler, ölçme planı, seçenekler, üretim kodu, iptaller ve anahtar düzeltmeleri, madde analizi girdileri) gzip ile sıkıştırılmış tek bir JSON dosyasına yazar. **Kayıtlı çalışmayı aç** ile ya da dosyayı A kitapçığı alanına bırakarak iş kaldığı yerden sürer; kitapçıklar oluşturulmuşsa aynı üretim koduyla birebir yeniden üretilir. Dosya öğrenci cevaplarını içerebilir; yalnızca kullanıcının bilgisayarına iner.

## Ölçme planı ve ölçme sonuçları

2. adımdaki **Ölçme planı** panelinde dersin ve programın öğrenme çıktıları (DÖÇ, PÇ), Ders Bilgi Paketindeki DÖÇ-PÇ ilişki matrisi (0-5) ve her sorunun bilişsel düzeyi (Hatırlama, Anlama, Uygulama, Analiz, Değerlendirme, Yaratma) ile haftası girilir. Sorunun DÖÇ'ü listede seçilen ÖÇ'dür.

**Sınavdan önce** iki sayfalık, yatay A4 **Ölçme planı** yazdırılır (ya da PDF'e kaydedilir):
1. DÖÇ ve bilişsel düzeye göre A kitapçığı soru numaraları, soru sayısı ve puan,
2. puanlama ölçütleri,
3. sınavın PÇ'lere ortalama katkısı (1-5) ve düzeyi (3 altı düşük, 3-3,99 orta, 4 ve üstü yüksek),
4. soru, cevap, hafta, düzey, DÖÇ ve PÇ katkılarını gösteren soru-çıktı matrisi.

Bir sorunun PÇ katkısı, ölçtüğü DÖÇ'nün matristeki değeridir (birden çok DÖÇ varsa en yükseği); sınavın katkısı soruların ortalamasıdır.

**Sınavdan sonra**, madde analizinin altındaki **Ölçme sonuçları** aynı dört bölümü sonuçlarla doldurur: her hücrede başarı yüzdesi ve DÖÇ'ye ulaşma durumu; sınav istatistikleri (puan, puan dağılımı, KR-20, güçlük ve ayırt edicilik dağılımı); PÇ'ye planlanan katkı, katkı ağırlıklı başarı ve gerçekleşen katkı (planlanan × başarı oranı); soru bazında p, D ve karar (koru, gözden geçir, düzelt ya da çıkar, anahtarı kontrol et). Rapor yazdırılır ve CSV olarak iner. PÇ değerleri sınava dayalı bir göstergedir, PÇ'nin doğrudan ölçümü değildir.

Plan bilgileri cevap anahtarı dosyasına (`#PLAN` satırı) yazılır; ayrıca `.json` olarak kaydedilip sonraki dönem aynı ders için yeniden yüklenebilir. Örnek: [ornek/Ornek_Sinav_olcme-plani.json](ornek/Ornek_Sinav_olcme-plani.json).

## Kendi kurumunuza uyarlama (şablon)

Araç açık kaynaklıdır ve başka okullarda kullanılabilir. Kurum adı, logo, ana renk ve cevap anahtarı formunun doküman numarası iki yoldan değiştirilir:

- **Sayfadan:** en alttaki **Kurum ve görünüm ayarları** bölümünde üst satır, üniversite, birim, kısa ad, form doküman numarası ve yürürlük tarihi yazılır, ana renk seçilir, logo (PNG ya da JPG) yüklenir. Ayarlar yalnızca o tarayıcıda saklanır; **Ayar dosyasını indir** ile `.json` olarak alınıp başka bilgisayarda yüklenebilir.
- **Kalıcı olarak (fork):** `index.html` içindeki `HTMYO_KURUM_VARS` nesnesini düzenleyin:

```js
const HTMYO_KURUM_VARS={
  ust:'T.C.',
  univ:'ÜNİVERSİTENİZİN ADI',
  birim:'Fakülte ya da yüksekokul adı',
  kisa:'KISA AD',
  renk:'#3B2A8F',                       // arayüz ve Word başlık rengi
  logo:'data:image/png;base64,...',     // boş bırakılabilir
  logoW:114,logoH:200,                  // logonun piksel boyutu (oran için)
  p248No:'FORM-NO',p248Tarih:'GG.AA.YYYY',
  p248Not:'Cevap anahtarının teslimine ilişkin kurum notu.'
};
```

Bu bilgiler ölçme planı ve ölçme sonuçları raporlarının başlığına, PFRM-248 biçimindeki Sınav Cevap Anahtarı Word dosyasına ve sayfanın üst şeridine yazılır. Ana renk değişince arayüzün bütün tonları bu renkten türetilir. Sayfadaki "Yüksekokulumuzun şablonu" gibi kuruma özgü metinler ve şablon bağlantısı `index.html` içinde düz metin olarak durur; fork eden kurum bunları kendi metniyle değiştirebilir. Telif bildirimi ve atıf korunmalıdır.

## Özellikler

- Soruları ve şıkları karıştırır; görselli, öncüllü ve tablolu sorular bütün olarak taşınır.
- "Hepsi / Hiçbiri" gibi şıkları yerinde bırakabilir; iki şıklı (Doğru/Yanlış) soruları karıştırmaz.
- Klasik şablonda soru puanlarını puan tablosunda sorularla birlikte taşır.
- İstenirse aynı sıradaki sorunun doğru cevabını kitapçıklar arasında farklı harfe koyar (A kitapçığının 1. sorusunun cevabı B ise B, C, D, E kitapçıklarının 1. sorusunun cevabı B olmaz ve birbirini tekrar etmez); harf dağılımını da dengeler.
- Doğru cevapların şıklara dağılımını (hangi şıkta kaç doğru cevap olduğunu) her kitapçık için gösterir.
- Her dosyanın "Kitapçık türü" alanını kendi harfiyle doldurur.
- Cevap anahtarını ve soru eşleşme tablosunu yazdırılabilir ve CSV olarak verir. Yazdırılan anahtarda ders, sınav, tarih, öğretim elemanı ve imza alanı bulunur.
- **Soru blokları ve sabit sorular:** ortak metne bağlı ya da "yukarıdaki soruya göre" diye başlayan sorular birlikte taşınır; istenen soru yerinde sabit kalır.
- **Ardışık harf sınırı:** aynı cevap harfi en fazla 3 kez üst üste gelir.
- **Alt bilgi:** her sayfanın altına "B KİTAPÇIĞI · Sayfa 2 / 4" yazılır.
- **Gizlilik temizliği:** Word açıklamaları, gizli metin, yazar ve son kaydeden bilgisi silinir; izlenen değişiklikler kabul edilir.
- **Büyük puntolu kopya:** büyük puntolu soru kitapçığı hakkı olan öğrenciler için her kitapçığın ayrı bir kopyası; sorular, şıklar ve yönerge en az 18 punto ve tek sütun olur, form başlığı ve bilgi tabloları normal boyutta kalır.
- **Üretim kodu:** aynı dosya, aynı cevaplar, aynı seçenekler ve aynı kodla kitapçıklar birebir aynı yeniden üretilir.
- **Soru iptali ve anahtar düzeltme:** A'daki bir sorunun her kitapçıktaki yeri gösterilir; iptal ya da cevap değişikliği bütün anahtarlara tek seferde işlenir.
- **Öğrenme çıktıları (ÖÇ):** her sorunun ölçtüğü ÖÇ araçta seçilir; sorulara ve öğrenciye giden kitapçıklara ÖÇ yazılmaz. ÖÇ bilgisi ayrı olarak üretilen **PFRM-248 Sınav Cevap Anahtarı** Word dosyasına (Soru No, Beklenen cevap, Ölçülen DÖÇ, Puan; her kitapçık için ayrı tablo), cevap anahtarı tablosuna ve CSV dosyasına yazılır. Dosyadaki `[ÖÇ2]` notları ve Aiken'daki `OC: 2` satırları okunur ve kitapçıklardan silinir.
- **Öğrenme Çıktılarına Ulaşma tablosu:** madde analizinde her ÖÇ için soru sayısı, toplam puan, sınıfın başarı yüzdesi, hedefe ulaşan öğrenci sayısı ve oranı, Ulaşıldı/Ulaşılamadı durumu; eşik ayarlanabilir (varsayılan %60), iptal edilen sorular sayılmaz, birden çok ÖÇ'ye bağlı soru her birine tam sayılır. Tablo yazdırılır ve PFRM-250 Program Çıktıları Değerlendirme Formu'na aktarılacak düzende CSV olarak iner.
- **Bağlam yardımı:** her bölümün yanındaki **?** düğmesine basınca o bölümün ne işe yaradığını anlatan kısa bir pencere açılır; pencereden resimli yardımın ilgili başlığına geçilir.
- **Madde analizi:** optik okuyucu çıktısı (.txt, .csv, .xlsx) yüklenir; bütün kitapçıklar A sırasına çevrilir, her soru için güçlük (p), ayırt edicilik (D) ve çeldirici analizi, sınav için KR-20 güvenirliği hesaplanır; öğrenci puanları CSV olarak alınır. Cevaplar anahtarla uyuşmuyor görünüyorsa (şans düzeyinde ortalama, negatif KR-20, yaygın anahtar hatası notu, kitapçıklar arasında büyük fark) kırmızı uyarı verir.

## Sürüm notları

**2.2.0 (16 Kasım 2026).** Ölçme planı ve ölçme sonuçları, kurum şablonu:
- 2. adımda **Ölçme planı** paneli: ders ve sınav bilgileri, DÖÇ ve PÇ metinleri, DÖÇ-PÇ matrisi (Excel'den yapıştırılabilir), soru başına bilişsel düzey ve hafta (toplu giriş), puanlama ölçütleri; plan dosyası (.json) kaydetme ve yükleme.
- Sınav öncesi iki sayfalık, yatay A4 **Ölçme planı** çıktısı.
- Madde analizinden sonra aynı düzende **Ölçme sonuçları** çıktısı ve CSV dosyası.
- Plan bilgisi cevap anahtarı dosyasına yazılır ve madde analizinde okunur; eski anahtar dosyaları için plan dosyası ayrıca yüklenebilir.
- **Kurum ve görünüm ayarları:** kurum adı, logo, ana renk, form numarası; tarayıcıda saklanır, .json olarak dışa ve içe aktarılır. PFRM-248 dosyası bu ayarlarla üretilir. Fork için `HTMYO_KURUM_VARS`.
- **Önceki sürümler:** 1.0.0'dan 2.1.0'a kadar eski sürümler `surumler/` klasöründe çalışır halde durur; sayfanın altındaki sürüm numarasından açılır.
- **Çalışmayı kaydet (.htmyo):** yüklenen A kitapçığı, cevaplar, ÖÇ'ler, ölçme planı, seçenekler, üretim kodu, iptal ve anahtar düzeltmeleri ve madde analizi girdileri tek dosyaya kaydedilir; dosya açılınca kitapçıklar aynı kodla birebir yeniden üretilir ve iş kaldığı yerden sürer. Kaydedilmemiş çalışmada sayfa kapatılırken uyarı verilir.
- Yeni yardım bölümleri ve ekran görüntüleri; örnek ölçme planı dosyası.

Önceki sürümlerle uyumludur: üretim kodları aynı kitapçıkları verir, eski cevap anahtarı dosyaları okunur; plan girilmezse araç önceki gibi çalışır.

**2.1.0 (14 Kasım 2026).** Madde analizinde eşleşme denetimi: sınıf ortalaması şans düzeyine yakınsa, KR-20 negatifse, soruların yarısından fazlasında "anahtar hatası olabilir" notu varsa ya da kitapçık türleri arasında ortalama doğru farkı 2 kat ve üstündeyse sonuçların en üstünde ve ÖÇ tablosunun üstünde kırmızı uyarı çıkar. Sonuç başlığında anahtar dosyasının üretim kodu büyük yazılır. Düzeltmeler:
- Excel'de açılıp virgül ya da sekmeyle veya tırnaklı olarak yeniden kaydedilen cevap anahtarı dosyaları okunur; okunamayan dosya için "0 soru" yerine açık bir hata verilir.
- Bütün soruları boş bırakan öğrenci analize katılır.
- Optik dosyada soru sayısından fazla cevap varsa ve iptal kutusuna sınavda olmayan bir numara yazılırsa uyarı verilir.
- Optik Excel dosyasındaki başlık satırı "okunamayan satır" sayılmaz.
- Telefonda sayfanın yana taşması giderildi (ÖÇ toplu giriş ve ÖÇ raporu alanları).
- Anahtar dosyası yüklenince üretim kodu da gösterilir; aynı dosya yeniden seçilebilir.

**2.0.0 (14 Kasım 2026).** Araç kitapçık karıştırmanın yanında sınav belgelendirme ve akreditasyon işini de üstlenir:
- Öğrenme çıktıları (ÖÇ) seçimi; ÖÇ'ler öğrenciye giden kitapçıklara yazılmaz.
- Ayrı **PFRM-248 Sınav Cevap Anahtarı** Word dosyası; cevap anahtarında ve CSV dosyasında ÖÇ bilgisi.
- Madde analizinde **Öğrenme Çıktılarına Ulaşma** tablosu (PFRM-250 için yazdırma ve CSV).
- Her bölümde **?** yardım düğmeleri.

Önceki sürümlerle uyumludur: eski üretim kodları aynı kitapçıkları verir, eski cevap anahtarı dosyaları okunmaya devam eder; ÖÇ seçmeyen kullanıcı için araç önceki gibi çalışır.

**1.x.** Soru blokları ve sabit sorular, soru iptali ve anahtar düzeltme, alt bilgi, gizlilik temizliği, büyük puntolu kopya, ardışık harf sınırı, üretim kodu, madde analizi, metin dosyası (Aiken) girişi.

## Güvenlik ve gizlilik

- Sorular hiçbir sunucuya gönderilmez; tüm işlem tarayıcıda yapılır.
- Sayfa, İçerik Güvenliği Politikası (CSP) ile hiçbir adrese bağlanamayacak, form gönderemeyecek ve dışarıdan kod yükleyemeyecek şekilde kilitlenmiştir. Dış kütüphane kullanılmaz.
- Aracı yalnızca resmi bağlantıdan (yukarıdaki adres ya da yüksekokulun web sitesindeki bağlantı) açın. E-posta veya mesajla gönderilen başka kopyaları kullanmayın.

## Atıf

Bu yazılım MIT Lisansı ile yayımlanmıştır. Kullanan, değiştiren veya dağıtan herkes telif bildirimini korumalı ve şu atfı vermelidir:

> Çetin, B. (2026). *Kitapçık Oluşturucu* (Sürüm 2.2.0) [Yazılım]. Zenodo. https://doi.org/10.5281/zenodo.24226187

DOI (bütün sürümler, her zaman en son sürüme gider): [10.5281/zenodo.24226187](https://doi.org/10.5281/zenodo.24226187) · Sürüm 2.1.0: [10.5281/zenodo.24226188](https://doi.org/10.5281/zenodo.24226188) · Kaynak kod: https://github.com/behiccetin/htmyo-kitapcik

© 2026 Behiç ÇETİN
