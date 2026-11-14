# Kitapçık Oluşturucu

**Burdur Mehmet Akif Ersoy Üniversitesi, Bucak Hikmet Tolunay Ulaştırma ve Lojistik Meslek Yüksekokulu**

Yüksekokulun Sınav Soruları Formu (PFRM-217) ya da kendi Word dosyanızla hazırladığınız A kitapçığından, soruların ve şıkların yeri değiştirilmiş **B, C, D ve E kitapçıklarını** ve her birinin **cevap anahtarını** üreten, tek dosyalık web aracı.

**Kullanmak için:** https://behiccetin.github.io/htmyo-kitapcik/

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

```
1. Aşağıdakilerden hangisi bir taşıma türüdür?
A) Depolama
B) Karayolu
C) Paketleme
D) Etiketleme
E) Sayım
```

## Özellikler

- Soruları ve şıkları karıştırır; görselli, öncüllü ve tablolu sorular bütün olarak taşınır.
- "Hepsi / Hiçbiri" gibi şıkları yerinde bırakabilir; iki şıklı (Doğru/Yanlış) soruları karıştırmaz.
- Klasik şablonda soru puanlarını puan tablosunda sorularla birlikte taşır.
- Her dosyanın "Kitapçık türü" alanını kendi harfiyle doldurur.
- Cevap anahtarını ve soru eşleşme tablosunu yazdırılabilir ve CSV olarak verir.

## Güvenlik ve gizlilik

- Sorular hiçbir sunucuya gönderilmez; tüm işlem tarayıcıda yapılır.
- Sayfa, İçerik Güvenliği Politikası (CSP) ile hiçbir adrese bağlanamayacak, form gönderemeyecek ve dışarıdan kod yükleyemeyecek şekilde kilitlenmiştir. Dış kütüphane kullanılmaz.
- Aracı yalnızca resmî bağlantıdan (yukarıdaki adres ya da yüksekokulun web sitesindeki bağlantı) açın. E-posta veya mesajla gönderilen başka kopyaları kullanmayın.

## Atıf

Bu yazılım MIT Lisansı ile yayımlanmıştır. Kullanan, değiştiren veya dağıtan herkes telif bildirimini korumalı ve şu atfı vermelidir:

> Çetin, B. (2026). *Kitapçık Oluşturucu* (Sürüm 1.0.0) [Yazılım]. Burdur Mehmet Akif Ersoy Üniversitesi Bucak Hikmet Tolunay Ulaştırma ve Lojistik Meslek Yüksekokulu. https://github.com/behiccetin/htmyo-kitapcik

© 2026 Behiç ÇETİN
