# Memory Bank & Constitutional AI Agent System 🧠

[English](docs/README.en.md) | [Türkçe](docs/README.tr.md) | [Azərbaycan](docs/README.az.md) | [Deutsch](docs/README.de.md) | [Français](docs/README.fr.md) | [Español](docs/README.es.md)

> Determinist çərçivə: LLM-ləri vəziyyətsiz (stateless), sənəd yönümlü proqram mühəndislərinə çevirmək üçün.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Əsas Fəlsəfə

Təsəvvür edin ki, mükəmməl memarlıq intizamına malik bir ekspert proqramçı var — lakin hər sessiyadan sonra **tam yaddaş itkisi** yaşayır.  
Onun işləməsi yalnız iki sənədə əsaslanır:

1. **Constitution (`AGENTS-Constitution.md`)**  
   Layihənin dəyişməz texniki qanunu.

2. **Memory Bank (`MemoryBank.md` + context faylları)**  
   Məqsədlərin, memarlığın, qərarların və inkişafın canlı, versiyalaşdırılmış qeydi.

Bu məhdudiyyət bir üstünlüyə çevrilir:

> **Mükəmməl sənədləşmə · Təkrarlana bilən məntiq · Memarlıq əsaslı inkişaf**

---

## 📁 Depo Quruluşu

```text
memory-bank/
├── MemoryBank.md           # Əməliyyat protokolu & RAGESe framework
├── AGENTS-Constitution.md  # Ali texniki qanun (dəyişməz qaydalar)
├── projectbrief.md         # Strateji “niyə” və uğur meyarları
├── productContext.md       # İstifadəçi problemləri & təcrübə məqsədləri
├── systemPatterns.md       # Memarlıq & dizayn şablonları
├── techContext.md          # Texnoloji yığın, alətlər, məhdudiyyətlər
├── activeContext.md        # Cari vəziyyət & fokus
└── progress.md             # İnkişaf jurnalı & qərar tarixi

🚀 Sürətli Başlanğıc
1️⃣ Layihəyə Klon Et

git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank

2️⃣ Constitution-u Fərdiləşdir

memory-bank/AGENTS-Constitution.md faylını redaktə et:

    Dil və versiya parametrlərini dəyiş

    Memarlıq qatlarını müəyyən et

    Kod keyfiyyəti, test və dizayn qaydalarını tənzimlə

    ⚠️ Bu fayl layihə qanunudur. Dəyişiklikləri diqqətlə et.

3️⃣ Konteksti Başlat

İlk növbədə bu faylları doldur:

    projectbrief.md — Layihənin mövcudluq səbəbi

    techContext.md — İstifadə olunan texnologiyalar

    systemPatterns.md — Memarlıq və sərhədlər

🤖 İlk Prompt — Boot Protocol

AI agenti başlatmaq üçün tam olaraq bu prompt-dan istifadə et:

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

🔄 Gündəlik İş Prompt-u

As per MemoryBank.md protocol:

- Re-read all Memory Bank files
- Re-anchor to project goals and AGENTS-Constitution.md

TASK: [Tapşırığın təsviri]

CONSTITUTIONAL ARTICLES INVOLVED:
- Art. X — [Qayda adı]
- Art. Y — [Qayda adı]

Execute the task.

Before completion:
1. Pass the Context Integrity Gateway
2. Update:
   - activeContext.md (Son dəyişikliklər)
   - progress.md (Qərar jurnalı)
3. Confirm full constitutional compliance

Final response MUST include:
- Implementation summary
- Compliance confirmation
- Exact documentation updates

🧩 RAGESe Protokolu
Addım	Cavablandırılan sual	Hərəkət
Retrieve	Nə bilirəm?	Bütün Memory Bank fayllarını oxu
Anchor	Nə dəyişməzdir?	Məqsədlərə & Constitution-a sabitlən
Ground	İndi nə realdır?	Faktiki kodu və vəziyyəti yoxla
Evaluate	Uyğundurmu?	Qaydalara və memarlığa qarşı yoxla
Synthesize	Nə qurulmalıdır?	Həll yarat
evolve	Necə xatırlayacağıq?	Memory Bank-i yenilə
🛡️ Context Integrity Gateway

Hər hansı sənəd yeniləməsindən əvvəl:

    Fayllararası yoxlama — Ziddiyyət olmamalıdır

    Qərar qeydləri — Səbəb progress.md faylında saxlanılmalıdır

    Anomaliya eskalasiyası — Sənədləşdirilməmiş reallıqlar bildirilməlidir

Bu mexanizm memarlıq sürüşməsinə qarşı sistemin “immun reaksiyasıdır”.
📋 Nümunə İş Axını — Xüsusiyyət Əlavə Etmə

Ssenari: “Parol sıfırlama” funksiyasını əlavə et

1. İstifadəçi tapşırığı verir  
2. Agent RAGESe-ni icra edir:
   - Memory Bank-i oxuyur
   - Constitution-u yoxlayır
   - Əvvəl interfeysi dizayn edir
   - Testləri və implementasiyanı yazır
   - Sənədləri yeniləyir
3. Agent Context Integrity Gateway-dən keçir
4. Agent kodu + yaddaş yeniləmələrini təqdim edir

🎖️ Ən Yaxşı Təcrübələr

    Kiçik və aydın addımlarla başla

    Constitution-u erkən fərdiləşdir

    Anomaliya aşkarlanmasına etibar et

    progress.md faylını mütəmadi yoxla

    Sürətdən çox aydınlığa üstünlük ver

🔧 Uyğunlaşdırma Bələdçisi
Python olmayan layihələr

    Constitution-da runtime/alət hissələrini dəyiş

    techContext.md faylını yenilə

Müxtəlif Memarlıqlar

    Constitution-da qatları yenidən təyin et

    systemPatterns.md ilə uyğunlaşdır

    Asılılıq qaydalarını qoruyun

Xüsusi Qaydalar Əlavə Etmə

    Yeni konstitusiya maddələri əlavə et

    Onları Memory Bank və Gateway-də istinad et

❓ FAQ

Hər dəfə uzun prompt yazmalıyam?
Xeyr. İlk başlanğıcdan sonra qısa, protokol əsaslı prompt-lar kifayətdir.

Ən yaxşı modellər hansılardır?
Geniş konteks pəncərəsinə malik modellər (GPT-4+, Claude 3.5+ və s.).

Clean Architecture məcburidirmi?
Xeyr. Vacib olan ardıcıllıqdır — konkret bir memarlıq deyil.

Böyük layihələr üçün uyğundurmu?
Bəli. Hierarxik Memory Bank faylları və xülasələr vasitəsilə miqyaslana bilər.
🤝 Töhfə Vermə

Qarşıladığımız töhfələr:

    Digər dillər üçün Constitution faylları (Go, Rust, TypeScript və s.)

    Avtomatlaşdırma və bootstrap alətləri

    Real dünya nümunələri

Daha ətraflı üçün CONTRIBUTING.md sənədinə bax.
📜 Lisenziya

MIT Lisenziyası — ətraflı məlumat üçün LICENSE sənədinə bax.