# PTDXF

# Protected Trusted Document Exchange Format

PTDXF is a secure, auditable and trusted document exchange format designed for organizations, governments, critical infrastructures and regulated industries.

Unlike traditional document formats, PTDXF stores only visible information and excludes active, hidden, linked or executable content by design.

---

## Official Definition

**PTDXF (Protected Trusted Document Exchange Format)** is a standardized document format for secure document exchange, compliance and long-term archiving.

PTDXF stores visible information only and fundamentally excludes active, hidden, linked, embedded or executable content.

Non-compliant content shall be removed during document creation and validated again during document opening.

Violations that can be safely removed shall be sanitized automatically.

Manipulations that cannot be safely sanitized shall result in document rejection.

---

## Mission

PTDXF enables trusted document exchange by limiting document contents to visible information only.

Documents are sanitized during export and validated again before display.

---

## Core Principle

> What would not be visible on a printed document shall neither be stored nor displayed in a PTDXF document.

---

## Key Features

### Security by Design

- No macros
- No JavaScript
- No ActiveX
- No executable content
- No embedded files
- No forms
- No scripts
- No external resources

### Trusted Exchange

- Sanitized document export
- Secure document validation
- Optional digital signatures
- Audit-friendly structure

### Compliance Support

Suitable for:

- ISO 27001 environments
- TISAX environments
- Government agencies
- Critical infrastructure operators
- Regulated industries
- Long-term archiving

### AI-Friendly Design

PTDXF uses a structured document model to improve machine interpretation.

Optional image classifications may be provided:

- photo
- technical_drawing
- electrical_schematic
- blueprint
- process_diagram
- flow_chart
- table_scan

---

## Allowed Content

PTDXF supports only:

### Pages

Static document pages.

### Text

Visible UTF-8 text content.

Supported formatting:

- Bold
- Italic
- Underline

### Images

Supported image formats:

- JPEG
- PNG

Image metadata shall be removed during export.

---

## Forbidden Content

PTDXF documents shall not contain:

- Macros
- VBA
- JavaScript
- ActiveX
- Forms
- Embedded files
- Audio
- Video
- 3D objects
- Comments
- Change tracking
- Version history
- Hyperlinks
- External references
- Network resources
- Cloud references
- Executable content

---

## Security Levels

### LEVEL 0 – Trusted

The document fully complies with the PTDXF specification.

Action:

- Open document
- Display document

### LEVEL 1 – Sanitized

Removable violations have been detected.

Examples:

- Hyperlinks
- Metadata
- Comments

Action:

- Remove violations
- Revalidate document
- Display sanitized document

### LEVEL 2 – Critical Security Violation

The document contains non-removable or unknown structures.

Examples:

- Unknown object types
- Structural manipulation
- Invalid binary blocks
- Integrity violations

Action:

- Deny document opening
- Deny document display

Optional:

- Create forensic text extraction

---

## Forensic Extraction

For LEVEL 2 documents only.

Generated filename:

```text
<DocumentName>_(potentially_malicious).txt
```

File format:

```text
UTF-8
```

Purpose:

- Security investigations
- Incident response
- Malware analysis
- Forensic review

---

## File Extension

```text
.ptdxf
```

Proposed MIME Type:

```text
application/ptdxf
```

---

## Object Model

PTDXF recognizes only three object types:

```text
Page
Text
Image
```

Any other object type is considered non-compliant.

---

## Positioning

PTDXF is not intended to replace PDF, DOCX or ODT.

PTDXF complements existing document formats as a:

- Security format
- Exchange format
- Compliance format
- Audit format
- Archiving format

for trusted document content.

---

## Repository Structure

```text
/specification
/examples
/schemas
/compliance
/branding
/reader
/converter
```

---

## Roadmap

### Phase 1

- PTDXF Specification
- PTDXF Reference Reader
- PDF to PTDXF Converter
- DOCX to PTDXF Converter

### Phase 2

- Digital Signatures
- Validation Suite
- Compliance Certification

### Phase 3

- Linux Support
- Android Support
- iOS Support
- Enterprise Integrations

---

## Motto

### Visible Information. Nothing More.

### What is not visible shall not exist.

---

## License

Specification License: TBD

Reference Implementations: TBD

---
