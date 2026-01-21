# Medication Snapshot - Project Reference

> **Purpose:** Central reference document for AI assistants and developers working on this project. Keep this updated as the project evolves.

---

## 🎯 Project Overview

**Medication Snapshot** is an Android app that lets users photograph medication prescriptions, automatically extract information using AI/OCR, and maintain a digital medication record with an accessibility-first UI.

### Core Value Proposition
> "The simplest way to digitize prescriptions"

### Primary Differentiator
AI-powered prescription scanning — major competitors (Medisafe, MyTherapy, Dosecast) focus on reminders but **none offer automatic text extraction from prescription images**.

---

## 👥 Target Users

| Segment | Size (US) | Key Need |
|---------|-----------|----------|
| Self-managing patients | - | Quick, accurate prescription digitization |
| Elderly patients (65+) | 54M+ | Simple, accessible UI with large text/buttons |
| Family caregivers | 53M+ | Organized records for doctor visits |

---

## ✅ Key Decisions Made

| Decision | Choice | Rationale |
|----------|--------|-----------|
| **Data Storage** | Local SQLite | Privacy-first, offline access |
| **Monetization** | Free app | Focus on adoption, no barriers |
| **Platform** | Android only (v1) | Prioritize single platform quality |
| **UI Framework** | Jetpack Compose | Modern, declarative UI |
| **OCR Primary** | Google ML Kit | Free, on-device, privacy |
| **OCR Fallback** | Cloud Vision API | Higher accuracy for edge cases |
| **Accessibility** | WCAG 2.1 AA target | Serve underserved elderly market |

---

## 🔑 Critical Requirements

### Must-Have for v1
1. **Camera/gallery image capture** with preview
2. **AI text extraction** (medication name, dosage, frequency)
3. **Manual correction UI** for OCR errors
4. **Medication dashboard** with card-based layout
5. **Local SQLite storage** with encryption

### Accessibility (Non-Negotiable)
| Requirement | Specification |
|-------------|---------------|
| Touch targets | Minimum 48x48dp |
| Body text | Minimum 16sp |
| Headers | Minimum 20sp |
| Navigation depth | Maximum 3 levels |
| Contrast mode | High contrast option required |
| Error handling | Undo actions, confirmation dialogs |

---

## 🚫 Out of Scope (v1)

- Medication reminders/notifications
- PDF/CSV export
- Multi-user profiles
- Cloud backup/sync
- Drug interaction checking
- Voice input
- iOS version

---

## 📁 Project Documents

| Document | Path | Purpose |
|----------|------|---------|
| **BRD** | `brain/.../business_requirement_document.md` | Business requirements, stakeholder decisions |
| **Market Research** | `brain/.../market_research.md` | Competitive analysis, pain points |
| **PRD** | `brain/.../product_requirement_document.md` | Detailed product specs, features, wireframes |
| **Tech Spec** | `brain/.../technical_specification_document.md` | Architecture, data models, implementation details |
| **Task Tracker** | `brain/.../task.md` | Current progress checklist |

---

## 🏗️ Technical Stack

```
Platform:     Android 8.0+ (API 26+)
Language:     Kotlin
Architecture: MVVM + Clean Architecture
UI:           Jetpack Compose
Database:     Room + SQLCipher (encrypted)
OCR:          Google ML Kit (primary)
DI:           Hilt
Image:        CameraX, Coil
```

---

## 📊 Success Metrics

| Metric | Target |
|--------|--------|
| OCR Accuracy (printed) | > 85% |
| Scan Success Rate | > 90% |
| Time to Add Medication | < 30 seconds |
| User Retention (30-day) | > 60% |
| App Launch Time | < 3 seconds |

---

## 🎨 Design Principles

1. **Simplicity over features** — Avoid feature bloat
2. **Forgiving UI** — Always allow corrections, provide undo
3. **Progressive disclosure** — Show basic info first, details on demand
4. **Offline-first** — Core features work without internet
5. **Accessibility-first** — Design for elderly users, benefits everyone

---

## 📝 Development Guidelines

### Code Style
- Follow official Kotlin style guide
- Use meaningful variable/function names
- Document public APIs
- Write unit tests for business logic

### Git Workflow
- Feature branches from `main`
- Descriptive commit messages
- PR reviews before merge

### Testing Requirements
- Unit tests for ViewModels and Use Cases
- UI tests for critical user flows
- OCR accuracy tests with sample prescriptions

---

## 🔄 Update Log

| Date | Update |
|------|--------|
| 2026-01-21 | Initial project setup, BRD, Market Research, PRD created |

---

*Last updated: January 21, 2026*
