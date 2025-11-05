# Apple App Store Gizlilik Gereksinimleri - QR Master

Bu doküman, QR Master uygulamanızı Apple App Store'a gönderirken gereken gizlilik bilgilerini içerir.

## 📋 App Store Connect'te Doldurulacak Gizlilik Bilgileri

### 1. Data Collection (Veri Toplama)

App Store Connect'te "App Privacy" bölümünde aşağıdaki şekilde doldurmalısınız:

**Soru: Does your app collect data?**
**Cevap: NO** ✅

Hiçbir veri toplamadığınız için "No" seçeneğini işaretleyeceksiniz.

### 2. Privacy Policy URL

Apple, gizlilik politikası URL'i ister. Aşağıdaki seçeneklerden birini kullanabilirsiniz:

**Seçenek 1: GitHub Pages (ÖNERİLEN)**
```
https://batuhanaydin.github.io/qr-master.github.io/privacy.html
```

**Seçenek 2: Kendi domain'iniz**
```
https://yourdomain.com/privacy.html
```

### 3. Gizlilik Politikasını Yayınlama

#### GitHub Pages ile:

1. GitHub reposuna `privacy.html` dosyasını yükleyin
2. Repository Settings > Pages bölümüne gidin
3. Source: main branch seçin
4. Save yapın
5. URL otomatik olarak oluşur: `https://batuhanaydin.github.io/qr-master.github.io/privacy.html`

#### Komutlar:
```bash
cd qr-master
git add privacy.html privacy-policy-tr.md privacy-policy-en.md
git commit -m "Add privacy policy"
git push origin main
```

## 📱 App Store Connect - Privacy Details

### Data Types - Yanıtlar

| Kategori | Toplanan mı? | Açıklama |
|----------|--------------|----------|
| Contact Info | ❌ NO | Email, isim, telefon TOPLANIYOR MU? HAYIR |
| Health & Fitness | ❌ NO | Sağlık verileri TOPLANIYOR MU? HAYIR |
| Financial Info | ❌ NO | Ödeme bilgileri TOPLANIYOR MU? HAYIR |
| Location | ❌ NO | Konum TOPLANIYOR MU? HAYIR |
| Sensitive Info | ❌ NO | Hassas bilgi TOPLANIYOR MU? HAYIR |
| Contacts | ❌ NO | Kişiler TOPLANIYOR MU? HAYIR |
| User Content | ❌ NO | Kullanıcı içeriği TOPLANIYOR MU? HAYIR |
| Browsing History | ❌ NO | Tarama geçmişi TOPLANIYOR MU? HAYIR |
| Search History | ❌ NO | Arama geçmişi TOPLANIYOR MU? HAYIR |
| Identifiers | ❌ NO | Tanımlayıcılar TOPLANIYOR MU? HAYIR |
| Purchases | ❌ NO | Satın almalar TOPLANIYOR MU? HAYIR |
| Usage Data | ❌ NO | Kullanım verileri TOPLANIYOR MU? HAYIR |
| Diagnostics | ❌ NO | Hata raporları TOPLANIYOR MU? HAYIR |
| Other Data | ❌ NO | Diğer veriler TOPLANIYOR MU? HAYIR |

**TÜM SORULARA "NO" CEVABI VERİLECEK** ✅

## 🎯 App Description (Uygulama Açıklaması)

App Store'da kullanabileceğiniz açıklama:

### Türkçe:
```
QR Master - Hızlı ve Güvenli QR Kod Uygulaması

✨ ÖZELLİKLER:
• QR kod oluşturma
• QR kod tarama
• Geçmiş kayıtları
• Tamamen ücretsiz

🔒 GİZLİLİK:
• Hiçbir veri toplama yok
• Hesap gerektirmiyor
• Reklam yok
• Takip yok
• Verileriniz cihazınızda kalır

Gizliliğiniz bizim önceliğimizdir!
```

### İngilizce:
```
QR Master - Fast and Secure QR Code App

✨ FEATURES:
• Create QR codes
• Scan QR codes
• History records
• Completely free

🔒 PRIVACY:
• No data collection
• No account required
• No ads
• No tracking
• Your data stays on your device

Your privacy is our priority!
```

## 🛡️ Permission Usage Descriptions (İzin Açıklamaları)

Info.plist dosyanıza eklenecek:

```xml
<key>NSCameraUsageDescription</key>
<string>QR kodları taramak için kamera erişimi gereklidir. Görüntüler kaydedilmez.</string>

<key>NSCameraUsageDescription</key>
<string>Camera access is required to scan QR codes. Images are not recorded.</string>

<key>NSPhotoLibraryAddUsageDescription</key>
<string>QR kodları fotoğraf galerisine kaydetmek için izin gereklidir.</string>

<key>NSPhotoLibraryAddUsageDescription</key>
<string>Permission is required to save QR codes to photo gallery.</string>
```

## ✅ Checklist (Kontrol Listesi)

- [ ] `privacy.html` dosyasını GitHub'a yükle
- [ ] GitHub Pages'i aktif et
- [ ] Privacy policy URL'ini test et
- [ ] App Store Connect'te "No data collection" seç
- [ ] Tüm privacy sorularına "NO" cevabı ver
- [ ] Privacy policy URL'ini App Store Connect'e ekle
- [ ] Info.plist'e permission descriptions ekle
- [ ] App açıklamasında gizlilik özelliklerini vurgula

## 📧 İletişim Bilgisi

App Store Connect'te support URL ve email adresi istenir:

**Support Email:** your@email.com ← Kendi emailinizi ekleyin
**Privacy Policy URL:** https://batuhanaydin.github.io/qr-master.github.io/privacy.html

## 🎉 Son Notlar

QR Master uygulamanız hiçbir veri toplamadığı için Apple'ın gizlilik onayını kolayca alacaktır. Bu, kullanıcılar için büyük bir avantajdır ve App Store'da güven oluşturur.

Başarılar! 🚀
