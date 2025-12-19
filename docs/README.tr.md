# Bellek Bankası & Anayasal YZ Ajan Sistemi 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> LLM'leri vatansız, dokümantasyon odaklı yazılım mühendislerine dönüştürmek için deterministik bir çerçeve.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Temel Felsefe

Her oturumdan sonra tam hafıza kaybı yaşayan, mükemmel mimari disipline sahip uzman bir geliştirici hayal edin.
İşlev görebilmek için **tamamen** iki şeye güvenir:

1.  **Bir Anayasa (`AGENTS-Constitution.md`)**
    Projenin tartışılmaz teknik yasası.

2.  **Bir Bellek Bankası (`MemoryBank.md` + bağlam dosyaları)**
    Hedeflerin, mimarinin, kararların ve ilerlemenin yaşayan, sürümlendirilmiş bir kaydı.

Bu kısıtlama bir süper güce dönüşür:

> **Mükemmel dokümantasyon · Tekrarlanabilir mantık yürütme · Önce mimari yaklaşımı**

---

## 📁 Depo Yapısı

```text
memory-bank/
├── MemoryBank.md           # Operasyonel protokol & RAGESe çerçevesi
├── AGENTS-Constitution.md  # Üstün teknik yasa (tartışılmaz kurallar)
├── projectbrief.md         # Stratejik "neden" ve başarı kriterleri
├── productContext.md       # Kullanıcı sorunları & deneyim hedefleri
├── systemPatterns.md       # Mimari & tasarım desenleri
├── techContext.md          # Teknoloji yığını, araçlar, kısıtlamalar
├── activeContext.md        # Mevcut durum & odak
└── progress.md             # Evrim günlüğü & karar geçmişi
```

---

## 🚀 Hızlı Başlangıç

### 1️⃣ Projenize Klonlayın

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Anayasayı Özelleştirin

`memory-bank/AGENTS-Constitution.md` dosyasını düzenleyin:

- Dil/çalışma zamanı sürümlerini ayarlayın
- Mimari katmanları tanımlayın
- Kod kalitesi, test ve tasarım kurallarını belirleyin

> ⚠️ Bu dosya **proje yasası** işlevi görür. Bilerek ve isteyerek değiştirin.

### 3️⃣ Bağlamınızı Başlatın

Önce bunları doldurun:

- `projectbrief.md` — Proje neden var
- `techContext.md` — Gerçek teknoloji yığını
- `systemPatterns.md` — Mimari & sınırlar

---

## 🤖 İlk İstem — Önyükleme Protokolü

Bir YZ ajanını başlatmak için **tam olarak** bu istemi kullanın:

```text
Vatansız bir yürütme modeli altında çalışıyorsunuz.

ADIM 1 — ZORUNLU BAĞLAM YÜKLEMESİ
`memory-bank/` dizininden aşağıdaki dosyaları okuyun ve içselleştirin:
1. MemoryBank.md
2. AGENTS-Constitution.md

Her ikisi de tamamen okunana kadar ilerlemeyin.

ADIM 2 — ONAY
Açıkça onaylayın:
- Her iki dosyayı da okudunuz ve anladınız
- RAGESe'yi, Bağlam Bütünlüğü Ağ Geçidi'ni ve anayasal otoriteyi kabul ediyorsunuz
- Belgelenmemiş hiçbir bilgi varsaymayacaksınız

ADIM 3 — PROJE ANALİZİ
Mevcut kod tabanını tarayın.
Bu dosyaların var olup olmadığını ve doğru olup olmadığını belirleyin:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

ADIM 4 — SENTEZ
Eksik veya güncel olmayan her dosya için:
- Oluşturma veya güncelleme önerin
- İçeriği kesinlikle gözlemlenebilir kod ve yapılandırmadan türetin
- Gereksinimler veya mimari İCAT ETMEYİN

ADIM 5 — AĞ GEÇİDİ
Dokümantasyonu geliştirmeden önce:
- Bağlam Bütünlüğü Ağ Geçidi'ni geçin
- Anormallikleri onay için yükseltin

Henüz kod yazmayın.

YALNIZCA şunlarla yanıt verin:
1. Uyumluluk onayı
2. Dokümantasyon sentez planı
```

---

## 🔄 Günlük Çalışma İstemi

```text
MemoryBank.md protokolü uyarınca:

- Tüm Bellek Bankası dosyalarını yeniden okuyun
- Proje hedeflerine ve AGENTS-Constitution.md'ye yeniden bağlanın

GÖREV: [Görevi tanımlayın]

İLGİLİ ANAYASAL MADDELER:
- Madde X — [Kural adı]
- Madde Y — [Kural adı]

Görevi yürütün.

Tamamlamadan önce:
1. Bağlam Bütünlüğü Ağ Geçidi'ni geçin
2. Güncelleyin:
   - activeContext.md (Son Değişiklikler)
   - progress.md (Karar Günlüğü)
3. Tam anayasal uyumluluğu onaylayın

Son yanıt ŞUNLARI İÇERMELİDİR:
- Uygulama özeti
- Uyumluluk onayı
- Kesin dokümantasyon güncellemeleri
```

---

## 🧩 RAGESe Protokolü

| Adım       | Cevaplanan Soru          | Eylem                                    |
|------------|--------------------------|------------------------------------------|
| Retrieve   | Ne biliyorum?            | TÜM Bellek Bankası dosyalarını oku       |
| Anchor     | Neyin değişemeyeceği?    | Hedeflere & Anayasaya kilitlen           |
| Ground     | Şu anda gerçek olan ne?  | Gerçek kodu & durumu incele              |
| Evaluate   | Bu uyuyor mu?            | Kuralları & mimariyi kontrol et          |
| Synthesize | Ne inşa edilmeli?        | Çözüm üret                               |
| evolve     | Nasıl hatırlıyoruz?      | Bellek Bankasını güncelle                |

---

## 🛡️ Bağlam Bütünlüğü Ağ Geçidi

Herhangi bir dokümantasyon evriminden önce:

- **Dosyalar arası doğrulama** — Çelişkilere izin verilmez
- **Karar günlüğü** — Gerekçeler `progress.md` içine kaydedilir
- **Anormallik yükseltme** — Belgelenmemiş gerçeklik işaretlenmelidir

Bu, mimari sapmalara karşı sistemin bağışıklık tepkisidir.

---

## 📋 Örnek İş Akışı — Özellik Ekleme

```text
Senaryo: "Şifre sıfırlama" özelliği ekle

1. Kullanıcı görev istemini verir
2. Ajan RAGESe'yi yürütür:
   - Bellek Bankasını okur
   - Anayasayı doğrular
   - Önce arayüz çözümünü tasarlar
   - Testleri ve uygulamayı yazar
   - Dokümantasyonu günceller
3. Ajan Bağlam Bütünlüğü Ağ Geçidi'ni geçer
4. Ajan kodu + hafıza güncellemelerini teslim eder
```

---

## 🎖️ En İyi Uygulamalar

- Küçük ve açık başlayın
- Anayasayı erkenden özelleştirin
- Anormallik tespitine güvenin
- `progress.md` dosyasını düzenli olarak inceleyin
- Hız yerine netliği tercih edin

---

## 🔧 Uyarlama Kılavuzu

### Python Olmayan Projeler
- Anayasa çalışma zamanı/araçlar bölümlerini değiştirin
- `techContext.md` dosyasını buna göre güncelleyin

### Farklı Mimariler
- Anayasa'daki katmanları yeniden tanımlayın
- `systemPatterns.md` dosyasını hizalayın
- Bağımlılık kurallarını koruyun

### Özel Kurallar Ekleme
- Yeni anayasal maddeler ekleyin
- Bunlara Bellek Bankası & Ağ Geçidi'nde referans verin

---

## ❓ SSS

**Her seferinde uzun istemlere ihtiyacım var mı?**
Hayır. Önyüklemeden sonra, kısa protokol tabanlı istemler yeterlidir.

**Hangi modeller en iyi çalışır?**
Geniş bağlam pencerelerine sahip modeller (GPT-4+, Claude 3.5+, vb.).

**Temiz Mimari (Clean Architecture) zorunlu mu?**
Hayır. Tutarlılık zorunludur — belirli bir mimari değil.

**Bu büyük projelere ölçeklenebilir mi?**
Evet. Hiyerarşik Bellek Bankası dosyaları ve özetleri kullanın.

---

## 🤝 Katkıda Bulunma

Şunları memnuniyetle karşılıyoruz:
- Diğer diller için Anayasalar (Go, Rust, TypeScript)
- Otomasyon & önyükleme araçları
- Gerçek dünya vaka çalışmaları

Bkz. `CONTRIBUTING.md`.

---

## 📜 Lisans

MIT Lisansı — bkz. `LICENSE`.
