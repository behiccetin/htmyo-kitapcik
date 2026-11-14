# Kitapçık Oluşturucu

**Burdur Mehmet Akif Ersoy Üniversitesi, Bucak Hikmet Tolunay Ulaştırma ve Lojistik Meslek Yüksekokulu**

Yüksekokulun Sınav Soruları Formu (PFRM-217), kendi Word dosyanız ya da bir metin dosyasıyla (.txt, Aiken biçimi dahil) hazırladığınız A kitapçığından, soruların ve şıkların yeri değiştirilmiş **B, C, D ve E kitapçıklarını** ve her birinin **cevap anahtarını** üreten, tek dosyalık web aracı.

**Kullanmak için:** https://behiccetin.github.io/htmyo-kitapcik/

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
- **Madde analizi:** optik okuyucu çıktısı (.txt, .csv, .xlsx) yüklenir; bütün kitapçıklar A sırasına çevrilir, her soru için güçlük (p), ayırt edicilik (D) ve çeldirici analizi, sınav için KR-20 güvenirliği hesaplanır; öğrenci puanları CSV olarak alınır.

## Güvenlik ve gizlilik

- Sorular hiçbir sunucuya gönderilmez; tüm işlem tarayıcıda yapılır.
- Sayfa, İçerik Güvenliği Politikası (CSP) ile hiçbir adrese bağlanamayacak, form gönderemeyecek ve dışarıdan kod yükleyemeyecek şekilde kilitlenmiştir. Dış kütüphane kullanılmaz.
- Aracı yalnızca resmî bağlantıdan (yukarıdaki adres ya da yüksekokulun web sitesindeki bağlantı) açın. E-posta veya mesajla gönderilen başka kopyaları kullanmayın.

## Atıf

Bu yazılım MIT Lisansı ile yayımlanmıştır. Kullanan, değiştiren veya dağıtan herkes telif bildirimini korumalı ve şu atfı vermelidir:

> Çetin, B. (2026). *Kitapçık Oluşturucu* (Sürüm 1.3.0) [Yazılım]. Burdur Mehmet Akif Ersoy Üniversitesi Bucak Hikmet Tolunay Ulaştırma ve Lojistik Meslek Yüksekokulu. https://github.com/behiccetin/htmyo-kitapcik

© 2026 Behiç ÇETİN
