# Development Rules

> **Version:** 0.1.0
> **Status:** Draft

---

# Purpose

Dokumen ini berisi aturan dasar yang harus diikuti selama pengembangan SimCH Engine.

Seluruh kontribusi, baik dari manusia maupun AI Assistant, wajib mengikuti aturan yang tercantum dalam dokumen ini agar proyek tetap konsisten, mudah dipelihara, dan dapat berkembang dalam jangka panjang.

---

# Rule 1 — Documentation First Development (DFD)

Semua fitur baru wajib diawali dengan dokumentasi sebelum implementasi kode.

Urutan pengembangan:

```
Idea
    ↓
Documentation
    ↓
Discussion
    ↓
Architecture
    ↓
Implementation
    ↓
Testing
```

Tidak diperbolehkan langsung menulis kode tanpa dokumentasi.

---

# Rule 2 — Domain Driven Design (DDD)

Seluruh sistem harus dibangun berdasarkan domain bisnis, bukan berdasarkan framework atau teknologi.

Contoh:

```
World
NPC
Economy
Building
Quest
Simulation
Weather
Combat
```

Bukan:

```
Controllers
Managers
Helpers
Utils
```

Domain adalah pusat dari seluruh arsitektur.

---

# Rule 3 — Clean Architecture

Dependency selalu mengarah ke dalam.

```
UI
 ↓
Application
 ↓
Domain
 ↑
Infrastructure
```

Domain tidak boleh mengetahui implementasi framework.

---

# Rule 4 — Plugin First

Semua fitur harus dirancang agar dapat dipisahkan menjadi plugin apabila diperlukan.

Engine inti harus tetap kecil dan modular.

---

# Rule 5 — Data Driven

Sebisa mungkin seluruh konfigurasi disimpan dalam data.

Contoh:

* JSON
* YAML
* Database
* Script
* Asset

Hindari nilai yang di-hardcode di dalam source code.

---

# Rule 6 — Single Responsibility

Setiap class, module, maupun package hanya memiliki satu tanggung jawab utama.

Jika sebuah file memiliki terlalu banyak fungsi, maka file tersebut harus dipecah.

---

# Rule 7 — Low Coupling, High Cohesion

Setiap module harus:

* Memiliki tanggung jawab yang jelas.
* Tidak bergantung secara berlebihan pada module lain.
* Mudah diganti tanpa memengaruhi sistem lain.

---

# Rule 8 — Convention Over Configuration

Gunakan struktur proyek yang konsisten.

Jangan membuat banyak konfigurasi jika sebuah konvensi sudah cukup.

---

# Rule 9 — Naming Convention

Gunakan nama yang mudah dipahami.

Contoh:

```
SimulationWorld
EconomySystem
NPCBehavior
QuestEngine
```

Hindari nama seperti:

```
Manager1
Helper2
TempData
NewSystem
```

Nama harus menjelaskan tujuan objek.

---

# Rule 10 — Folder Convention

Folder mengikuti domain.

Contoh:

```
world/
economy/
npc/
combat/
simulation/
editor/
```

Bukan berdasarkan jenis file semata.

---

# Rule 11 — Git Commit Convention

Format commit:

```
feat:
fix:
docs:
refactor:
test:
style:
build:
ci:
perf:
chore:
```

Contoh:

```
feat: add economy simulation
docs: update project vision
fix: resolve npc movement bug
```

---

# Rule 12 — Code Quality

Kode harus:

* Mudah dibaca.
* Mudah diuji.
* Mudah dipelihara.
* Menghindari duplikasi.

Prinsip:

> Write code for humans first, computers second.

---

# Rule 13 — AI Collaboration

AI digunakan sebagai partner pengembangan, bukan pengganti pengembang.

AI dapat membantu:

* Brainstorming
* Dokumentasi
* Refactoring
* Testing
* Code Generation

Namun keputusan akhir tetap berada di tangan maintainer proyek.

---

# Rule 14 — Backward Compatibility

Perubahan besar harus mempertimbangkan kompatibilitas terhadap sistem yang sudah ada.

Breaking change harus didokumentasikan dengan jelas.

---

# Rule 15 — Long-Term Thinking

Setiap keputusan teknis harus mempertimbangkan dampaknya dalam jangka panjang.

Hindari solusi cepat yang dapat menambah utang teknis (technical debt).

---

# Development Workflow

Standar alur kerja pengembangan:

```
Idea
    ↓
Documentation
    ↓
Discussion
    ↓
Architecture
    ↓
Implementation
    ↓
Testing
    ↓
Review
    ↓
Merge
```

---

# Core Principles

Seluruh pengembangan SimCH Engine harus selalu mengacu pada prinsip berikut:

* Documentation First
* Domain First
* Simulation First
* AI Native
* Plugin First
* Data Driven
* Clean Architecture
* Maintainability
* Scalability
* Reusability

---

# Final Statement

Development Rules bukan sekadar pedoman teknis, tetapi fondasi budaya pengembangan SimCH Engine.

Setiap kontribusi diharapkan mengikuti prinsip-prinsip ini agar SimCH Engine tetap konsisten, modular, dan mampu berkembang dalam jangka panjang.
