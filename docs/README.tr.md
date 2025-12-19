# Memory Bank & Constitutional AI Agent System 🧠

[English](docs/README.en.md) | [Türkçe](docs/README.tr.md) | [Azərbaycan](docs/README.az.md) | [Deutsch](docs/README.de.md) | [Français](docs/README.fr.md) | [Español](docs/README.es.md)

> Deterministik bir çerçeve: LLM’leri stateless, dokümantasyon odaklı yazılım mühendislerine dönüştürmek için.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Temel Felsefe

Mükemmel mimari disiplini olan bir uzman geliştirici düşünün — ancak her oturumdan sonra **tam hafıza kaybı** yaşıyor.  
Bu geliştirici işlevini yalnızca iki yapıya borçludur:

1. **Constitution (`AGENTS-Constitution.md`)**  
   Projenin tartışılmaz teknik yasası.

2. **Memory Bank (`MemoryBank.md` + context dosyaları)**  
   Hedeflerin, mimarinin, kararların ve ilerlemenin yaşayan, versiyonlanmış kaydı.

Bu kısıtlama bir süper güce dönüşür:

> **Mükemmel dokümantasyon · Yeniden üretilebilir mantık · Mimari öncelikli geliştirme**

---

## 📁 Depo Yapısı

```text
memory-bank/
├── MemoryBank.md           # Operasyonel protokol & RAGESe framework’ü
├── AGENTS-Constitution.md  # Yüce teknik yasa (değiştirilemez kurallar)
├── projectbrief.md         # Stratejik “neden” ve başarı kriterleri
├── productContext.md       # Kullanıcı problemleri & deneyim hedefleri
├── systemPatterns.md       # Mimari & tasarım kalıpları
├── techContext.md          # Teknoloji yığını, araçlar, kısıtlar
├── activeContext.md        # Güncel durum & odak noktası
└── progress.md             # Evrim günlüğü & karar geçmişi

🚀 Hızlı Başlangıç
1️⃣ Projeye Klonla

git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank

2️⃣ Constitution’u Özelleştir

memory-bank/AGENTS-Constitution.md dosyasını düzenle:

    Dil/sürüm bilgilerini ayarla

    Mimari katmanları tanımla

    Kod kalitesi, test ve tasarım kurallarını belirle

    ⚠️ Bu dosya proje yasasıdır. Değişiklikleri bilinçli yap.

3️⃣ Bağlamı (Context) Başlat

Öncelikle şu dosyaları doldur:

    projectbrief.md — Projenin varlık nedeni

    techContext.md — Kullanılan teknoloji yığını

    systemPatterns.md — Mimari yapı ve sınırlar

🤖 İlk Prompt — Boot Protocol

AI ajanını başlatmak için tam olarak şu prompt’u kullan:

You are operating under a stateless execution model.

STEP 1 — MANDATORY CONTEXT LOAD
Read and internalize the following files from the `memory-bank/` directory:
1. MemoryBank.md
2. AGENTS-Constitution.md

Do not proceed until both are fully read.

STEP 2 — ACKNOWLEDGEMENT
Explicitly confirm:
- You have read and understood both files
- You accept RAGESe, the Context Integrity Gateway, and constitutional authority
- You will assume no undocumented knowledge

STEP 3 — PROJECT ANALYSIS
Scan the existing codebase.
Identify whether these files exist and are accurate:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

STEP 4 — SYNTHESIS
For each missing or outdated file:
- Propose creation or update
- Derive content strictly from observable code and config
- Do NOT invent requirements or architecture

STEP 5 — GATEWAY
Before evolving documentation:
- Pass the Context Integrity Gateway
- Escalate anomalies for confirmation

Do NOT write code yet.

Respond ONLY with:
1. Compliance confirmation
2. Documentation synthesis plan

🔄 Günlük Çalışma Prompt’u

As per MemoryBank.md protocol:

- Re-read all Memory Bank files
- Re-anchor to project goals and AGENTS-Constitution.md

TASK: [Görev açıklaması]

CONSTITUTIONAL ARTICLES INVOLVED:
- Art. X — [Kural adı]
- Art. Y — [Kural adı]

Execute the task.

Before completion:
1. Pass the Context Integrity Gateway
2. Update:
   - activeContext.md (Son değişiklikler)
   - progress.md (Karar günlüğü)
3. Confirm full constitutional compliance

Final response MUST include:
- Implementation summary
- Compliance confirmation
- Exact documentation updates

🧩 RAGESe Protokolü
Adım	Cevaplanan Soru	Eylem
Retrieve	Ne biliyorum?	Tüm Memory Bank dosyalarını oku
Anchor	Ne değişemez?	Hedeflere & Constitution’a sabitlen
Ground	Şu anda ne gerçek?	Gerçek kodu & durumu incele
Evaluate	Bu uygun mu?	Kurallar & mimariyle doğrula
Synthesize	Ne inşa edilmeli?	Çözümü üret
evolve	Nasıl hatırlayacağız?	Memory Bank’i güncelle
🛡️ Context Integrity Gateway

Herhangi bir dokümantasyon evriminden önce:

    Dosyalar arası doğrulama — Çelişki olmamalı

    Karar kaydı — Gerekçe progress.md içinde tutulmalı

    Anomali yükseltme — Belirlenmemiş gerçeklikler rapor edilmeli

Bu mekanizma, mimari sapmaya (architectural drift) karşı sistemin bağışıklığıdır.
📋 Örnek Akış — Bir Özellik Ekleme

Senaryo: "Şifre sıfırlama" özelliğini ekle

1. Kullanıcı görevi belirtir
2. Agent RAGESe’yi çalıştırır:
   - Memory Bank’i okur
   - Constitution’u doğrular
   - Önce arayüz tasarımıyla çözümü oluşturur
   - Testleri ve implementasyonu yazar
   - Dokümantasyonu günceller
3. Agent Context Integrity Gateway’den geçer
4. Agent kodu + bellek güncellemelerini teslim eder

🎖️ En İyi Uygulamalar

    Küçük ve açık adımlarla başla

    Constitution’u erken özelleştir

    Anomali tespitine güven

    progress.md dosyasını düzenli gözden geçir

    Hızdan ziyade açıklığa öncelik ver

🔧 Uyarlama Rehberi
Python Dışı Projeler

    Constitution’daki runtime/araç bölümlerini değiştir

    techContext.md dosyasını güncelle

Farklı Mimariler

    Constitution’daki katmanları yeniden tanımla

    systemPatterns.md ile hizala

    Bağımlılık kurallarını koru

Özel Kurallar Ekleme

    Yeni anayasal maddeler ekle

    Bunları Memory Bank & Gateway içinde referansla

❓ SSS

Her seferinde uzun prompt mu yazmam gerekiyor?
Hayır. İlk başlatmadan sonra kısa, protokol tabanlı prompt’lar yeterlidir.

Hangi modeller en uygunudur?
Büyük context penceresine sahip modeller (GPT-4+, Claude 3.5+, vb.).

Clean Architecture zorunlu mu?
Hayır. Zorunlu olan tutarlılıktır — belirli bir mimari değil.

Bu sistem büyük projelere ölçeklenebilir mi?
Evet. Hiyerarşik Memory Bank dosyaları ve özetler kullanarak ölçeklenebilir.
🤝 Katkıda Bulunma

Şunları memnuniyetle kabul ediyoruz:

    Diğer diller için Constitution’lar (Go, Rust, TypeScript, vb.)

    Otomasyon & bootstrap araçları

    Gerçek dünya vaka çalışmaları

Ayrıntılar için CONTRIBUTING.md dosyasına bak.
📜 Lisans

MIT Lisansı — ayrıntılar için LICENSE dosyasına bak.