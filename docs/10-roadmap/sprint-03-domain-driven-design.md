# Sprint 03 — Domain Driven Design (DDD)

> **Status:** ⬜ Not Started
> **Version:** v0.0.3
> **Estimated Duration:** 1–2 Weeks (Flexible)

---

# Objective

Mendefinisikan struktur Domain Driven Design (DDD) SimCH Engine sebagai fondasi seluruh arsitektur engine.

Sprint ini **belum membahas implementasi kode**, tetapi menentukan bagaimana dunia SimCH dibagi menjadi domain yang independen, mudah dikembangkan, dan mudah dipahami oleh manusia maupun AI.

---

# Deliverables

* Domain Map
* Bounded Context
* Ubiquitous Language
* Domain Dependency
* Domain Responsibility
* Domain Lifecycle
* Future Package Structure

---

# Phase 1 — Ubiquitous Language

## Objective

Menyatukan bahasa yang digunakan dalam seluruh proyek.

### Tasks

Buat file:

```text
docs/03-domain/ubiquitous-language.md
```

Isi:

* Agent
* Organization
* Simulation
* World
* Event
* Component
* System
* Domain
* Service
* Aggregate
* Entity
* Value Object

### Checklist

* [ ] Semua istilah memiliki definisi
* [ ] Tidak ada istilah ganda

### Output

Semua developer menggunakan bahasa yang sama.

---

# Phase 2 — Domain Identification

## Objective

Mengidentifikasi seluruh domain utama SimCH Engine.

### Tasks

Buat file:

```text
docs/03-domain/domain-map.md
```

Daftar domain awal:

* Agent Domain
* World Domain
* Simulation Domain
* Organization Domain
* Economy Domain
* Conversation Domain
* Event Domain
* Resource Domain
* Rendering Domain
* Editor Domain
* Project Domain

### Checklist

* [ ] Semua domain teridentifikasi
* [ ] Domain memiliki deskripsi

### Output

Peta domain SimCH selesai.

---

# Phase 3 — Bounded Context

## Objective

Menentukan batas tanggung jawab setiap domain.

### Tasks

Buat file:

```text
docs/03-domain/bounded-context.md
```

Isi:

Untuk setiap domain jelaskan:

* Purpose
* Responsibility
* Owns
* Does Not Own
* Depends On

### Checklist

* [ ] Semua domain memiliki batas jelas

### Output

Tidak ada domain yang saling tumpang tindih.

---

# Phase 4 — Domain Relationship

## Objective

Menentukan hubungan antar domain.

### Tasks

Buat file:

```text
docs/03-domain/domain-relationship.md
```

Contoh:

```text
Agent
│
├── uses World
├── triggers Event
├── joins Organization
└── affects Economy
```

### Checklist

* [ ] Dependency Diagram selesai
* [ ] Hubungan domain terdokumentasi

### Output

Interaksi antar domain jelas.

---

# Phase 5 — Domain Responsibilities

## Objective

Menentukan tanggung jawab masing-masing domain.

### Tasks

Buat file:

```text
docs/03-domain/domain-responsibilities.md
```

Isi setiap domain:

* Responsibilities
* Inputs
* Outputs
* Events Produced
* Events Consumed

### Checklist

* [ ] Semua domain memiliki tanggung jawab

### Output

Setiap domain memiliki peran yang jelas.

---

# Phase 6 — Aggregate Design

## Objective

Menentukan Aggregate Root pada setiap domain.

### Tasks

Buat file:

```text
docs/03-domain/aggregate-design.md
```

Contoh:

Agent Domain

* Agent
* Memory
* Needs
* Relationship

Organization Domain

* Company
* Department
* Employee

### Checklist

* [ ] Aggregate Root selesai

### Output

Struktur bisnis setiap domain terdokumentasi.

---

# Phase 7 — Future Package Structure

## Objective

Merancang struktur package berdasarkan domain.

### Tasks

Buat file:

```text
docs/03-domain/package-structure.md
```

Contoh:

```text
packages/

agent/
world/
simulation/
organization/
economy/
conversation/
event/
renderer/
editor/
```

### Checklist

* [ ] Package Structure selesai

### Output

Blueprint struktur package tersedia.

---

# Phase 8 — Sprint Review

## Sprint Checklist

### Domain

* [ ] Ubiquitous Language
* [ ] Domain Map
* [ ] Bounded Context
* [ ] Domain Relationship
* [ ] Domain Responsibilities
* [ ] Aggregate Design
* [ ] Package Structure

---

# Sprint Success Criteria

Sprint dianggap selesai apabila:

* Seluruh domain utama telah diidentifikasi.
* Setiap domain memiliki tanggung jawab yang jelas.
* Hubungan antar domain terdokumentasi.
* Struktur package masa depan telah dirancang.
* Belum ada implementasi kode.

---

# Next Sprint

➡ **Sprint 04 — System Architecture**

Fokus:

* Clean Architecture
* Layer Architecture
* Event-Driven Architecture
* Plugin Architecture
* Modular Package Architecture
* Dependency Rules
* Data Flow
* Communication Flow
