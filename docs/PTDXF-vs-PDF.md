# PTDXF vs PDF

# Comparison

This document compares PTDXF (Protected Trusted Document Exchange Format) with Portable Document Format (PDF).

---

## Overview

| Feature | PTDXF | PDF |
|----------|----------|----------|
| Visible text | Yes | Yes |
| Images | Yes | Yes |
| Hyperlinks | No | Yes |
| JavaScript | No | Yes |
| Embedded Files | No | Yes |
| Forms | No | Yes |
| Multimedia | No | Yes |
| Macros | No | Limited / Possible through integrations |
| Metadata | Removed | Supported |
| External References | No | Supported |
| Active Content | No | Supported |
| Network Actions | No | Possible |
| Full Text Search | Yes | Yes |
| Digital Signatures | Yes | Yes |
| Audit Focus | High | Medium |
| Attack Surface | Low | Higher |

---

## Design Philosophy

### PDF

PDF was designed to reproduce documents across different devices and operating systems.

Primary focus:

- Document fidelity
- Rich features
- Advanced workflows

---

### PTDXF

PTDXF was designed for trusted document exchange.

Primary focus:

- Security
- Simplicity
- Auditability
- Compliance

---

## Security

### PDF

PDF may contain:

- Hyperlinks
- Embedded content
- JavaScript
- Attachments
- Forms
- Multimedia

These features provide flexibility but increase complexity.

---

### PTDXF

PTDXF intentionally excludes:

- Hyperlinks
- Scripts
- Active Content
- Embedded Files
- Forms
- External Resources

Only visible information is retained.

---

## Auditability

### PDF

Auditability depends heavily on:

- Reader implementation
- Content inspection
- Security tooling

---

### PTDXF

Auditability is built into the format.

Allowed content:

- Page
- Text
- Image

Everything else is prohibited.

---

## Compliance

### Typical PDF Usage

- Publishing
- Manuals
- Reports
- Contracts

---

### Typical PTDXF Usage

- Compliance-controlled exchange
- Government communication
- External supplier communication
- Audit documentation
- Secure archiving

---

## Threat Surface Comparison

| Threat | PDF | PTDXF |
|----------|----------|----------|
| Hidden Hyperlinks | Possible | Removed |
| Metadata Leakage | Possible | Removed |
| Embedded Files | Possible | Prohibited |
| JavaScript | Possible | Prohibited |
| External Resources | Possible | Prohibited |
| Dynamic Content | Possible | Prohibited |
| Active Content | Possible | Prohibited |

---

## Conclusion

PDF remains one of the most important document formats for publishing and document exchange.

PTDXF is not intended to replace PDF.

PTDXF complements PDF by providing a security-focused format designed for trusted exchange, compliance, auditing and long-term archiving.

---

## Core Principle

> What would not be visible on a printed document shall neither be stored nor displayed in a PTDXF document.
