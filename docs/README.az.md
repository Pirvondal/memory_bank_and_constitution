# Yaddaş Bankı & Konstitusiyalı Sİ Agent Sistemi 🧠

[Türkçe](README.tr.md) | [Azərbaycan](README.az.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md)

> DİM-ləri (Böyük Dil Modellərini) vatansız, sənədləşdirmə əsaslı proqram mühəndislərinə çevirmək üçün deterministik çərçivə.

[![Lisenziya: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PR-lər Qəbul edilir](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 Əsas Fəlsəfə

Hər sessiyadan sonra tam yaddaş itkisi yaşayan, lakin mükəmməl memarlıq intizamına malik bir ekspert proqramçı təsəvvür edin.
Fəaliyyət göstərmək üçün o, **tamamilə** iki artefakta güvənir:

1.  **Konstitusiya (`AGENTS-Constitution.md`)**
    Layihənin müzakirə olunmayan texniki qanunu.

2.  **Yaddaş Bankı (`MemoryBank.md` + kontekst faylları)**
    Hədəflərin, memarlığın, qərarların və irəliləyişin canlı, versiyalı qeydi.

Bu məhdudiyyət bir super gücə çevrilir:

> **Mükəmməl sənədləşdirmə · Təkrarlana bilən məntiq · Memarlıq yönümlü inkişaf**

---

## 📁 Repozitoriya Strukturu

```text
memory-bank/
├── MemoryBank.md           # Əməliyyat protokolu & RAGESe çərçivəsi
├── AGENTS-Constitution.md  # Ali texniki qanun (müzakirə olunmayan qaydalar)
├── projectbrief.md         # Strateji "niyə" və uğur meyarları
├── productContext.md       # İstifadəçi problemləri & təcrübə hədəfləri
├── systemPatterns.md       # Memarlıq & dizayn nümunələri
├── techContext.md          # Texnologiya steki, alətlər, məhdudiyyətlər
├── activeContext.md        # Cari vəziyyət & fokus
└── progress.md             # Təkamül jurnalı & qərar tarixçəsi
```

---

## 🚀 Tez Başlanğıc

### 1️⃣ Layihənizə Klonlayın

```bash
git clone https://github.com/Pirvondal/memory_bank_and_constitution.git
cp -r memory_bank_and_constitution/memory-bank ./memory-bank
```

### 2️⃣ Konstitusiyanı Fərdiləşdirin

`memory-bank/AGENTS-Constitution.md` faylını redaktə edin:

- Dil/icra mühiti versiyalarını tənzimləyin
- Memarlıq təbəqələrini təyin edin
- Kod keyfiyyəti, test və dizayn qaydalarını müəyyənləşdirin

> ⚠️ Bu fayl **layihə qanunu** rolunu oynayır. Onu şüurlu şəkildə dəyişdirin.

### 3️⃣ Kontekstinizi Başladın

İlk olaraq bunları doldurun:

- `projectbrief.md` — Layihə niyə mövcuddur
- `techContext.md` — Faktiki texnologiya steki
- `systemPatterns.md` — Memarlıq & sərhədlər

---

## 🤖 İlk Sorğu — Yükləmə Protokolu

Bir Sİ agentini başlatmaq üçün **dəqiq olaraq** bu sorğudan istifadə edin:

```text
Siz vatansız icra modeli altında fəaliyyət göstərirsiniz.

ADDIM 1 — MƏCBURİ KONTEKST YÜKLƏNMƏSİ
`memory-bank/` qovluğundan aşağıdakı faylları oxuyun və mənimsəyin:
1. MemoryBank.md
2. AGENTS-Constitution.md

Hər ikisi tam oxunmadan davam etməyin.

ADDIM 2 — TƏSDİQ
Açıq şəkildə təsdiqləyin:
- Hər iki faylı oxudunuz və anladınız
- RAGESe-ni, Kontekst Bütövlüyü Şlüzünü və konstitusiya səlahiyyətini qəbul edirsiniz
- Sənədləşdirilməmiş heç bir biliyi fərz etməyəcəksiniz

ADDIM 3 — LAYİHƏ ANALİZİ
Mövcud kod bazasını skan edin.
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

ADDIM 5 — ŞLÜZ
Sənədləşdirməni təkmilləşdirməzdən əvvəl:
- Kontekst Bütövlüyü Şlüzünü keçin
- Anomaliyaları təsdiq üçün yüksəldin

Hələ kod yazmayın.

YALNIZ bunlarla cavab verin:
1. Uyğunluq təsdiqi
2. Sənədləşdirmə sentez planı
```

---

## 🔄 Günlük İş Sorğusu

```text
MemoryBank.md protokoluna əsasən:

- Bütün Yaddaş Bankı fayllarını yenidən oxuyun
- Layihə hədəflərinə və AGENTS-Constitution.md-yə yenidən bağlanın

TAPŞIRIQ: [Tapşırığı təsvir edin]

ƏLAQƏLİ KONSTİTUSİYA MADDƏLƏRİ:
- Maddə X — [Qayda adı]
- Maddə Y — [Qayda adı]

Tapşırığı icra edin.

Tamamlamadan əvvəl:
1. Kontekst Bütövlüyü Şlüzünü keçin
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
| Retrieve   | Mən nə bilirəm?          | BÜTÜN Yaddaş Bankı fayllarını oxu        |
| Anchor     | Nə dəyişə bilməz?        | Hədəflərə & Konstitusiyaya bağlan        |
| Ground     | Hazırda real olan nədir? | Faktiki kodu & vəziyyəti yoxla           |
| Evaluate   | Bu uyğundurmu?           | Qaydaları & memarlığı yoxla              |
| Synthesize | Nə qurulmalıdır?         | Həll yolu yarat                          |
| evolve     | Necə xatırlayırıq?       | Yaddaş Bankını yenilə                    |

---

## 🛡️ Kontekst Bütövlüyü Şlüzü

Hər hansı sənədləşdirmə təkamülündən əvvəl:

- **Fayllararası doğrulama** — Ziddiyyətlərə icazə verilmir
- **Qərar jurnalı** — Əsaslandırmalar `progress.md`-də qeyd olunur
- **Anomaliya yüksəltmə** — Sənədləşdirilməmiş reallıq işarələnməlidir

Bu, memarlıq sapmalarına qarşı sistemin immunitet reaksiyasıdır.

---

## 📋 Nümunə İş Axını — Xüsusiyyət Əlavə Etmə

```text
Ssenari: "Şifrə sıfırlama" xüsusiyyəti əlavə et

1. İstifadəçi tapşırıq sorğusunu verir
2. Agent RAGESe-ni icra edir:
   - Yaddaş Bankını oxuyur
   - Konstitusiyanı doğrular
   - Əvvəlcə interfeys həllini dizayn edir
   - Testləri və tətbiqi yazır
   - Sənədləşdirməni yeniləyir
3. Agent Kontekst Bütövlüyü Şlüzünü keçir
4. Agent kodu + yaddaş yeniləmələrini təhvil verir
```

---

## 🎖️ Ən Yaxşı Təcrübələr

- Kiçik və açıq başlayın
- Konstitusiyanı erkən fərdiləşdirin
- Anomaliya aşkarlanmasına güvənin
- `progress.md` faylını mütəmadi olaraq nəzərdən keçirin
- Sürət əvəzinə aydınlığa üstünlük verin

---

## 🔧 Uyğunlaşdırma Bələdçisi

### Python Olmayan Layihələr
- Konstitusiya icra mühiti/alətlər bölmələrini dəyişdirin
- `techContext.md` faylını buna uyğun yeniləyin

### Fərqli Memarlıqlar
- Konstitusiyadakı təbəqələri yenidən təyin edin
- `systemPatterns.md` faylını uyğunlaşdırın
- Asılılıq qaydalarını qoruyun

### Xüsusi Qaydalar Əlavə Etmə
- Yeni konstitusiya maddələri əlavə edin
- Onlara Yaddaş Bankı & Şlüzdə istinad edin

---

## ❓ TVS (Tez-tez Verilən Suallar)

**Hər dəfə uzun sorğulara ehtiyacım varmı?**
Xeyr. Yükləmədən sonra, qısa protokol əsaslı sorğular kifayətdir.

**Hansı modellər ən yaxşı işləyir?**
Geniş kontekst pəncərələrinə malik modellər (GPT-4+, Claude 3.5+, və s.).

**Təmiz Memarlıq (Clean Architecture) məcburidirmi?**
Xeyr. Ardıcıllıq məcburidir — konkret bir memarlıq deyil.

**Bu böyük layihələrə miqyaslana bilərmi?**
Bəli. İyerarxik Yaddaş Bankı faylları və xülasələri istifadə edin.

---

## 🤝 Töhfə

Aşağıdakıları məmnuniyyətlə qəbul edirik:
- Digər dillər üçün Konstitusiyalar (Go, Rust, TypeScript)
- Avtomatlaşdırma & önyükleme alətləri
- Real dünya nümunələri

Bax: `CONTRIBUTING.md`.

---

## 📜 Lisenziya

MIT Lisenziyası — bax `LICENSE`.
