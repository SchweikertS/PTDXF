# PTDXF vs PDF/A

# Comparison

This document compares PTDXF with PDF/A.

---

## Overview

| Feature | PTDXF | PDF/A |
|----------|----------|----------|
| Long-Term Archiving | Yes | Yes |
| Full Text Search | Yes | Yes |
| Digital Signatures | Optional | Supported |
| Hyperlinks | Removed | Supported |
| Metadata | Removed | Required/Supported |
| Embedded Files | Prohibited | Limited |
| Forms | Prohibited | Possible depending on version |
| External References | Prohibited | Restricted |
| Scripts | Prohibited | Prohibited |
| Active Content | Prohibited | Generally prohibited |
| Audit Focus | Very High | High |
| Machine Simplicity | High | Medium |

---

## Purpose

### PDF/A

PDF/A is an ISO-standardized archival format designed to ensure long-term document preservation.

Primary goal:

- Future readability

---

### PTDXF

PTDXF is a security-focused exchange and archival format.

Primary goals:

- Trusted exchange
- Reduced attack surface
- Auditability
- Secure archiving

---

## Metadata

### PDF/A

Metadata is commonly used and often required.

Examples:

- Author
- Creation date
- Document identifiers
- Archival information

---

### PTDXF

Metadata not required for document use is removed.

Only information required for document integrity should remain.

---

## Hyperlinks

### PDF/A

Hyperlinks may be preserved.

---

### PTDXF

Hyperlinks are removed.

Only visible text remains.

---

## Security Philosophy

### PDF/A

Preserve document information.

---

### PTDXF

Preserve visible document information only.

---

## Approved Content

### PDF/A

Supports many PDF objects while restricting certain features.

---

### PTDXF

Supports only:

- Page
- Text
- Image

All other object types are invalid.

---

## Typical Usage

### PDF/A

- Archives
- Government records
- Legal document retention

---

### PTDXF

- Secure external communication
- Audit-controlled exchange
- Compliance processes
- Trusted partner exchange
- Secure document archiving

---

## Threat Surface Comparison

| Threat | PDF/A | PTDXF |
|----------|----------|----------|
| Hyperlink Abuse | Possible | Removed |
| Metadata Leakage | Possible | Minimized |
| Hidden Information | Possible | Restricted |
| Active Content | Mostly Restricted | Prohibited |
| Structural Complexity | Medium | Low |

---

## Conclusion

PDF/A focuses on preservation.

PTDXF focuses on preservation and trusted document exchange.

The formats can complement each other depending on organizational requirements.

---

## Core Principle

> PTDXF stores visible information only.
