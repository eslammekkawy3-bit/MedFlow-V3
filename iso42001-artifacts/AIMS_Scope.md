<div align="center">

# AI Management System Scope
### MedFlow v4.0 · AI Management System (AIMS)

<br>

[![Status](https://img.shields.io/badge/Status-ACTIVE-2ea44f?style=flat-square)]()
[![Version](https://img.shields.io/badge/Version-1%2E1-0052cc?style=flat-square)]()
[![ISO 42001](https://img.shields.io/badge/ISO_42001-Clause_4.3-7b2d8b?style=flat-square)]()

</div>

<br>

| Field | Detail |
|-------|--------|
| **Document ID** | MF-ISO-02 |
| **Version** | 1.1 |
| **Date** | 2026-02-21 |
| **Author** | Dr. Islam Mekawy |
| **Reviewer** | Dr. Islam Mekawy (Lead Researcher) |
| **Approver** | Dr. Islam Mekawy (AI Governance Lead) |
| **Classification** | CONFIDENTIAL – Internal Use Only |
| **ISO 42001 Clause** | Clause 4.3 – Determining the Scope of the AIMS |
| **Supersedes** | AIMS-4-3-001 v1.0 (2026-02-02) |

---


## 1. 📋 Introduction

This document defines the scope of the MedFlow V3 AI Management System (AIMS) research initiative. As a Personal Innovation Prototype (Non-Commercial), this project establishes boundaries for AI governance study and compliance framework demonstration.

---

## 2. 📌 Research Context

This Individual Research Lab project explores healthcare insurance AI decision support systems. The research demonstrates processing of synthetic medical records for academic study of ICD-10 coding and Saudi AR-DRG v9.0 classification methodologies.

---

## 3. 🔍 AI Systems in Scope

### <font color="#58a6ff">3.1 Document Processing Pipeline</font>

- Input validation and sanitization research
- PDF/DOCX/Image text extraction techniques
- Clinical narrative parsing methodologies

### <font color="#58a6ff">3.2 PII Scrubbing Engine</font>

- Local LLM processing research (Llama 3.2 3B via Ollama)
- Saudi-specific pattern detection (National ID, phone formats)
- Name and address redaction techniques

### <font color="#58a6ff">3.3 Clinical Intelligence Engine</font>

- Diagnosis extraction and normalization research
- ICD-10-CM/PCS code assignment automation
- Procedure identification methodologies

### <font color="#58a6ff">3.4 DRG Classification System</font>

- Saudi AR-DRG v9.0 grouper implementation study
- NPHIES integration endpoint design
- Length of stay optimization research

### <font color="#58a6ff">3.5 Decision Recommendation Engine</font>

- Google Gemini integration (Primary reasoning — gemini_client.py v2.0.0)
- NCEBM Evidence Scorer (Layer 3 — ncebm_scorer.py v1.2.0)
- Confidence scoring and escalation logic

---

## 4. ⚙️ External Interface Design

The research AIMS demonstrates interfaces with the following systems:

| System | Interface Type | Data Exchanged |
|--------|---------------|----------------|
| NPHIES (Simulated) | REST API Design | Pre-authorization request/response formats |
| Hospital EHR (Mock) | HL7 FHIR Study | Synthetic clinical documents |
| Claims System (Design) | Internal API Spec | DRG codes, decision outcomes |
| Audit Repository | SQLite/CSV | Immutable decision logs |

---

## 5. 📌 Exclusions

The following are explicitly excluded from research scope:

- Real patient data (synthetic only)
- Production deployment
- Commercial use or distribution
- Outpatient processing workflows
- Integration with live healthcare systems

---

## 6. 🛡️ Regulatory Compliance Study

This research studies compliance requirements within Saudi Arabia including:

- Saudi Data & AI Authority (SDAIA) AI Ethics Principles
- Council of Health Insurance (CHI) regulations
- SAMA Cybersecurity Framework alignment
- Personal Data Protection Law (PDPL) requirements
- Saudi AR-DRG v9.0 classification standards

---

## 7. 📌 Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2026-02-02 | Dr. Islam Mekawy | Initial issue. AIMS scope defined for MedFlow V3 research prototype. |
| 1.1 | 2026-02-21 | Dr. Islam Mekawy | Converted from .docx to .md (MF-ISO-02). Applied standard document control header. Synchronized: Llama 3.1 → 3.2; Section 3.5 Decision Engine updated from "Claude validation layer" to "NCEBM Evidence Scorer (Layer 3)" reflecting v4.0 governance architecture. |

---

*This document is part of the MedFlow V3 ISO 42001:2023 compliance portfolio.*

*End of Document*
