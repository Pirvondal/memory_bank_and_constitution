# Memory Bank & Constitutional AI Agent System 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> LLM'leri stateless (durumsuz), dokümantasyon odaklı yazılım mühendislerine dönüştürmek için deterministik bir framework.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Temel Felsefe

Her oturumdan sonra tam hafıza kaybı yaşayan, mükemmel mimari disipline sahip uzman bir geliştirici hayal edin.
İşlev görebilmek için **tamamen** iki şeye güvenir:

1.  **Bir Constitution (`AGENTS-Constitution.md`)**
    Projenin tartışılmaz teknik yasası.

2.  **Bir Memory Bank (`MemoryBank.md` + bağlam dosyaları)**
    Hedeflerin, mimarinin, kararların ve ilerlemenin yaşayan, sürümlendirilmiş bir kaydı.

Bu kısıtlama bir süper güce dönüşür:

> **Mükemmel dokümantasyon · Tekrarlanabilir mantık yürütme · Architecture-first development**

---

## 📁 Repository Yapısı

```text
memory-bank/
├── MemoryBank.md           # Operasyonel protokol & RAGESe framework'ü
├── AGENTS-Constitution.md  # Üstün teknik yasa (tartışılmaz kurallar)
├── projectbrief.md         # Stratejik "neden" ve başarı kriterleri
├── productContext.md       # Kullanıcı sorunları & deneyim hedefleri
├── systemPatterns.md       # Mimari & tasarım desenleri (patterns)
├── techContext.md          # Tech stack, araçlar, kısıtlamalar
├── activeContext.md        # Mevcut durum & odak
└── progress.md             # Evrim günlüğü & karar geçmişi
```

---

## 🚀 Quick Start

### 1️⃣ Projenize Klonlayın

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Constitution'ı Özelleştirin

`memory-bank/AGENTS-Constitution.md` dosyasını düzenleyin:

- Dil/runtime sürümlerini ayarlayın
- Mimari katmanları tanımlayın
- Kod kalitesi, test ve tasarım kurallarını belirleyin

> ⚠️ Bu dosya **proje yasası** işlevi görür. Bilerek ve isteyerek değiştirin.

### 3️⃣ Context'inizi Başlatın

Önce bunları doldurun:

- `projectbrief.md` — Proje neden var
- `techContext.md` — Gerçek tech stack
- `systemPatterns.md` — Mimari & sınırlar

---

## 🤖 İlk Prompt — Boot Protocol

Bir AI ajanını başlatmak için **tam olarak** bu prompt'u kullanın:

```text
Stateless bir execution model altında çalışıyorsunuz.

ADIM 1 — ZORUNLU CONTEXT LOAD
`memory-bank/` dizininden aşağıdaki dosyaları okuyun ve içselleştirin:
1. MemoryBank.md
2. AGENTS-Constitution.md

Her ikisi de tamamen okunana kadar ilerlemeyin.

ADIM 2 — ACKNOWLEDGEMENT (ONAY)
Açıkça onaylayın:
- Her iki dosyayı da okudunuz ve anladınız
- RAGESe'yi, Context Integrity Gateway'i ve constitutional otoriteyi kabul ediyorsunuz
- Belgelenmemiş hiçbir bilgi varsaymayacaksınız

ADIM 3 — PROJECT ANALYSIS
Mevcut codebase'i tarayın.
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
- İçeriği kesinlikle gözlemlenebilir kod ve konfigürasyondan türetin
- Gereksinimler veya mimari İCAT ETMEYİN

ADIM 5 — GATEWAY
Dokümantasyonu geliştirmeden önce:
- Context Integrity Gateway'i geçin
- Anormallikleri onay için yükseltin

Henüz kod yazmayın.

YALNIZCA şunlarla yanıt verin:
1. Uyumluluk onayı
2. Dokümantasyon sentez planı
```

---

## 🔄 Günlük Çalışma Prompt'u

```text
MemoryBank.md protokolü uyarınca:

- Tüm Memory Bank dosyalarını yeniden okuyun
- Proje hedeflerine ve AGENTS-Constitution.md'ye yeniden bağlanın

TASK: [Görevi tanımlayın]

İLGİLİ CONSTITUTIONAL MADDELER:
- Madde X — [Kural adı]
- Madde Y — [Kural adı]

Görevi yürütün.

Tamamlamadan önce:
1. Context Integrity Gateway'i geçin
2. Güncelleyin:
   - activeContext.md (Son Değişiklikler)
   - progress.md (Karar Günlüğü)
3. Tam constitutional uyumluluğu onaylayın

Son yanıt ŞUNLARI İÇERMELİDİR:
- Uygulama özeti
- Uyumluluk onayı
- Kesin dokümantasyon güncellemeleri
```

---

## 🧩 RAGESe Protokolü

| Adım       | Cevaplanan Soru          | Eylem                                    |
|------------|--------------------------|------------------------------------------|
| Retrieve   | Ne biliyorum?            | TÜM Memory Bank dosyalarını oku          |
| Anchor     | Neyin değişemeyeceği?    | Hedeflere & Constitution'a kilitlen      |
| Ground     | Şu anda gerçek olan ne?  | Gerçek kodu & durumu incele              |
| Evaluate   | Bu uyuyor mu?            | Kuralları & mimariyi kontrol et          |
| Synthesize | Ne inşa edilmeli?        | Çözüm üret                               |
| evolve     | Nasıl hatırlıyoruz?      | Memory Bank'ı güncelle                   |

---

## 🛡️ Context Integrity Gateway

Herhangi bir dokümantasyon evriminden önce:

- **Dosyalar arası doğrulama** — Çelişkilere izin verilmez
- **Karar günlüğü** — Gerekçeler `progress.md` içine kaydedilir
- **Anormallik yükseltme** — Belgelenmemiş gerçeklik işaretlenmelidir

Bu, mimari sapmalara karşı sistemin bağışıklık tepkisidir.

---

## 📋 Örnek Workflow — Özellik Ekleme

```text
Senaryo: "Şifre sıfırlama" özelliği ekle

1. Kullanıcı görev prompt'unu verir
2. Agent RAGESe'yi yürütür:
   - Memory Bank'ı okur
   - Constitution'ı doğrular
   - Önce arayüz çözümünü tasarlar
   - Testleri ve uygulamayı yazar
   - Dokümantasyonu günceller
3. Agent Context Integrity Gateway'i geçer
4. Agent kodu + memory güncellemelerini teslim eder
```

---

## 🎖️ Best Practices

- Küçük ve açık başlayın
- Constitution'ı erkenden özelleştirin
- Anormallik tespitine güvenin
- `progress.md` dosyasını düzenli olarak inceleyin
- Hız yerine netliği tercih edin

---

## 🔧 Uyarlama Kılavuzu

### Python Olmayan Projeler
- Constitution runtime/araçlar bölümlerini değiştirin
- `techContext.md` dosyasını buna göre güncelleyin

### Farklı Mimariler
- Constitution'daki katmanları yeniden tanımlayın
- `systemPatterns.md` dosyasını hizalayın
- Bağımlılık kurallarını koruyun

### Özel Kurallar Ekleme
- Yeni constitutional maddeler ekleyin
- Bunlara Memory Bank & Gateway'de referans verin

---

## ❓ SSS

**Her seferinde uzun prompt'lara ihtiyacım var mı?**
Hayır. Boot'tan sonra, kısa protokol tabanlı prompt'lar yeterlidir.

**Hangi modeller en iyi çalışır?**
Geniş context pencerelerine sahip modeller (GPT-4+, Claude 3.5+, vb.).

**Clean Architecture zorunlu mu?**
Hayır. Tutarlılık zorunludur — belirli bir mimari değil.

**Bu büyük projelere ölçeklenebilir mi?**
Evet. Hiyerarşik Memory Bank dosyaları ve özetleri kullanın.

---

## 🤝 Contributing

Şunları memnuniyetle karşılıyoruz:
- Diğer diller için Constitution'lar (Go, Rust, TypeScript)
- Otomasyon & boot araçları
- Gerçek dünya vaka çalışmaları

Bkz. `CONTRIBUTING.md`.

---

## 📜 License

MIT License — bkz. `LICENSE`.
