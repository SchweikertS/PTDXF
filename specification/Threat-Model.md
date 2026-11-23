# PTDXF Threat Model

## Purpose

This document defines the threats PTDXF is designed to mitigate.

---

## Protected Assets

- Document integrity
- Document authenticity
- Information confidentiality
- Auditability
- Long-term readability

---

## Threat Categories

### T-001 Macro Execution

Examples:

- VBA
- Office Macros
- Embedded Script Engines

Status:

Mitigated

Reason:

Macros are prohibited.

---

### T-002 Script Execution

Examples:

- JavaScript
- ActiveX
- PDF Actions

Status:

Mitigated

Reason:

Scripts are prohibited.

---

### T-003 Hyperlink Abuse

Examples:

- Phishing URLs
- Hidden redirects
- URL tracking

Status:

Mitigated

Reason:

Hyperlinks are removed during export.

---

### T-004 Embedded Files

Examples:

- ZIP
- EXE
- DOCX
- PDF attachments

Status:

Mitigated

Reason:

Embedded files are prohibited.

---

### T-005 Metadata Leakage

Examples:

- Author
- GPS location
- Camera information

Status:

Mitigated

Reason:

Metadata is removed.

---

### T-006 External Resource Loading

Examples:

- External images
- External media
- Cloud references

Status:

Mitigated

Reason:

External references are prohibited.

---

### T-007 Structural Manipulation

Examples:

- Undefined object types
- Invalid binary sections
- Format violations

Status:

Detected

Result:

LEVEL 2
