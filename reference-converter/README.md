# PTDXF Reference Converter

The PTDXF Reference Converter transforms existing document formats into PTDXF.

The converter applies sanitization rules during export.

The output document shall contain visible information only.

---

## Supported Input Formats

Planned:

- PDF
- DOCX
- PPTX

Future:

- XLSX
- ODT
- HTML

---

## Conversion Principle

Input Document

↓

Extract Visible Content

↓

Remove Non-Compliant Content

↓

Create PTDXF

---

## Removal Examples

Removed:

- Hyperlinks
- Scripts
- Comments
- Metadata
- Embedded Files
- Tracking Information

Preserved:

- Visible Text
- Visible Images
- Page Structure

---

## Objective

Generate a PTDXF document that conforms to PTDXF Specification 1.x.
