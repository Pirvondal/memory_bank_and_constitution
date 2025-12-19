# Memory Bank & Constitutional AI Agent System 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> LLM-ləri stateless (vətənsiz), sənədləşdirmə əsaslı proqram mühəndislərinə çevirmək üçün deterministik çərçivə.

[![Lisenziya: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PR-lər Qəbul edilir](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Əsas Fəlsəfə

Hər sessiyadan sonra tam yaddaş itkisi yaşayan, lakin mükəmməl memarlıq intizamına malik bir ekspert proqramçı təsəvvür edin.
Fəaliyyət göstərmək üçün o, **tamamilə** iki artefakta güvənir:

1.  **Bir Constitution (`AGENTS-Constitution.md`)**
    Layihənin müzakirə olunmayan texniki qanunu.

2.  **Bir Memory Bank (`MemoryBank.md` + kontekst faylları)**
    Hədəflərin, memarlığın, qərarların və irəliləyişin canlı, versiyalı qeydi.

Bu məhdudiyyət bir super gücə çevrilir:

> **Mükəmməl sənədləşdirmə · Təkrarlana bilən məntiq · Architecture-first development**

---

## 📁 Repozitoriya Strukturu

```text
memory-bank/
├── MemoryBank.md           # Operasyonel protokol & RAGESe çərçivəsi
├── AGENTS-Constitution.md  # Ali texniki qanun (müzakirə olunmayan qaydalar)
├── projectbrief.md         # Strateji "niyə" və uğur meyarları
├── productContext.md       # İstifadəçi problemləri & təcrübə hədəfləri
├── systemPatterns.md       # Memarlıq & dizayn nümunələri
├── techContext.md          # Texnologiya steki, alətlər, məhdudiyyətlər
├── activeContext.md        # Cari vəziyyət & fokus
└── progress.md             # Təkamül jurnalı & qərar tarixçəsi
```

---

## 🚀 Quick Start

### 1️⃣ Layihənizə Klonlayın

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Constitution-ı Fərdiləşdirin

`memory-bank/AGENTS-Constitution.md` faylını redaktə edin:

- Dil/runtime versiyalarını tənzimləyin
- Memarlıq təbəqələrini təyin edin
- Kod keyfiyyəti, test və dizayn qaydalarını müəyyənləşdirin

> ⚠️ Bu fayl **layihə qanunu** rolunu oynayır. Onu şüurlu şəkildə dəyişdirin.

### 3️⃣ Kontekstinizi Başladın

İlk olaraq bunları doldurun:

- `projectbrief.md` — Layihə niyə mövcuddur
- `techContext.md` — Faktiki texnologiya steki
- `systemPatterns.md` — Memarlıq & sərhədlər

---

## 🤖 İlk Prompt — Boot Protocol

Bir AI agentini başlatmaq üçün **dəqiq olaraq** bu prompt-dan istifadə edin:

```text
Siz stateless bir icra modeli altında fəaliyyət göstərirsiniz.

ADDIM 1 — MƏCBURİ KONTEKST YÜKLƏNMƏSİ
`memory-bank/` qovluğundan aşağıdakı faylları oxuyun və mənimsəyin:
1. MemoryBank.md
2. AGENTS-Constitution.md

Hər ikisi tam oxunmadan davam etməyin.

ADDIM 2 — TƏSDİQ (ACKNOWLEDGEMENT)
Açıq şəkildə təsdiqləyin:
- Hər iki faylı oxudunuz və anladınız
- RAGESe-ni, Context Integrity Gateway-i və constitutional səlahiyyəti qəbul edirsiniz
- Sənədləşdirilməmiş heç bir biliyi fərz etməyəcəksiniz

ADDIM 3 — LAYİHƏ ANALİZİ
Mövcud codebase-i skan edin.
Bu faylların mövcud olub-olmadığını və dəqiq olub-olmadığını müəyyənləşdirin:
- projectbrief.md
- productContext.md
- systemPatterns.md
- techContext.md
- activeContext.md
- progress.md

ADDIM 4 — SENTEZ
Çatışmayan və ya köhnəlmiş hər bir fayl üçün:
- Yaratma və ya yeniləmə təklif edin
- Məzmunu ciddi şəkildə müşahidə olunan kod və konfiqurasiyadan çıxarın
- Tələblər və ya memarlıq İCAD ETMƏYİN

ADDIM 5 — GATEWAY
Sənədləşdirməni təkmilləşdirməzdən əvvəl:
- Context Integrity Gateway-i keçin
- Anomaliyaları təsdiq üçün yüksəldin

Hələ kod yazmayın.

YALNIZ bunlarla cavab verin:
1. Uyğunluq təsdiqi
2. Sənədləşdirmə sentez planı
```

---

## 🔄 Günlük İş Prompt-u

```text
MemoryBank.md protokoluna əsasən:

- Bütün Memory Bank fayllarını yenidən oxuyun
- Layihə hədəflərinə və AGENTS-Constitution.md-yə yenidən bağlanın

TASK: [Tapşırığı təsvir edin]

ƏLAQƏLİ CONSTITUTIONAL MADDƏLƏR:
- Maddə X — [Qayda adı]
- Maddə Y — [Qayda adı]

Tapşırığı icra edin.

Tamamlamadan əvvəl:
1. Context Integrity Gateway-i keçin
2. Yeniləyin:
   - activeContext.md (Son Dəyişikliklər)
   - progress.md (Qərar Jurnalı)
3. Tam konstitusiya uyğunluğunu təsdiqləyin

Son cavab BUNLARI EHTİVA ETMƏLİDİR:
- İcra xülasəsi
- Uyğunluq təsdiqi
- Dəqiq sənədləşdirmə yeniləmələri
```

---

## 🧩 RAGESe Protokolu

| Addım      | Cavablandırılan Sual     | Fəaliyyət                                |
|------------|--------------------------|------------------------------------------|
| Retrieve   | Mən nə bilirəm?          | BÜTÜN Memory Bank fayllarını oxu         |
| Anchor     | Nə dəyişə bilməz?        | Hədəflərə & Constitution-a bağlan        |
| Ground     | Hazırda real olan nədir? | Faktiki kodu & vəziyyəti yoxla           |
| Evaluate   | Bu uyğundurmu?           | Qaydaları & memarlığı yoxla              |
| Synthesize | Nə qurulmalıdır?         | Həll yolu yarat                          |
| evolve     | Necə xatırlayırıq?       | Memory Bank-ı yenilə                     |

---

## 🛡️ Context Integrity Gateway

Hər hansı sənədləşdirmə təkamülündən əvvəl:

- **Fayllararası doğrulama** — Ziddiyyətlərə icazə verilmir
- **Qərar jurnalı** — Əsaslandırmalar `progress.md`-də qeyd olunur
- **Anomaliya yüksəltmə** — Sənədləşdirilməmiş reallıq işarələnməlidir

Bu, memarlıq sapmalarına qarşı sistemin immunitet reaksiyasıdır.

---

## 📋 Nümunə Workflow — Feature Əlavə Etmə

```text
Ssenari: "Şifrə sıfırlama" feature-u əlavə et

1. İstifadəçi tapşırıq prompt-unu verir
2. Agent RAGESe-ni icra edir:
   - Memory Bank-ı oxuyur
   - Constitution-ı doğrular
   - Əvvəlcə interfeys həllini dizayn edir
   - Testləri və tətbiqi yazır
   - Sənədləşdirməni yeniləyir
3. Agent Context Integrity Gateway-i keçir
4. Agent kodu + memory yeniləmələrini təhvil verir
```

---

## 🎖️ Best Practices

- Kiçik və açıq başlayın
- Constitution-ı erkən fərdiləşdirin
- Anomaliya aşkarlanmasına güvənin
- `progress.md` faylını mütəmadi olaraq nəzərdən keçirin
- Sürət əvəzinə aydınlığa üstünlük verin

---

## 🔧 Uyğunlaşdırma Bələdçisi

### Python Olmayan Layihələr
- Constitution runtime/alətlər bölmələrini dəyişdirin
- `techContext.md` faylını buna uyğun yeniləyin

### Fərqli Memarlıqlar
- Constitution-dakı təbəqələri yenidən təyin edin
- `systemPatterns.md` faylını uyğunlaşdırın
- Asılılıq qaydalarını qoruyun

### Xüsusi Qaydalar Əlavə Etmə
- Yeni constitutional maddələr əlavə edin
- Onlara Memory Bank & Gateway-də istinad edin

---

## ❓ FAQ

**Hər dəfə uzun prompt-lara ehtiyacım varmı?**
Xeyr. Boot-dan sonra, qısa protokol əsaslı prompt-lar kifayətdir.

**Hansı modellər ən yaxşı işləyir?**
Geniş context pencerelerine malik modellər (GPT-4+, Claude 3.5+, və s.).

**Clean Architecture məcburidirmi?**
Xeyr. Ardıcıllıq məcburidir — konkret bir memarlıq deyil.

**Bu böyük layihələrə miqyaslana bilərmi?**
Bəli. İyerarxik Memory Bank faylları və xülasələri istifadə edin.

---

## 🤝 Contributing

Aşağıdakıları məmnuniyyətlə qəbul edirik:
- Digər dillər üçün Constitution-lar (Go, Rust, TypeScript)
- Avtomatlaşdırma & boot alətləri
- Real dünya nümunələri

Bax: `CONTRIBUTING.md`.

---

## 📜 Lisenziya

MIT Lisenziyası — bax `LICENSE`.
