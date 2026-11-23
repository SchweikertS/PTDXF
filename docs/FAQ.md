# Frequently Asked Questions (FAQ)

# PTDXF – Protected Trusted Document Exchange Format

---

## What is PTDXF?

PTDXF (Protected Trusted Document Exchange Format) is a secure and auditable document exchange format designed for trusted document sharing, compliance, and long-term archiving.

PTDXF stores visible information only and excludes active, hidden, linked, embedded, or executable content by design.

---

## Why was PTDXF created?

Modern document formats often contain features that increase complexity and security risks.

Examples include:

- Macros
- JavaScript
- Embedded files
- Hyperlinks
- Metadata
- Forms
- External references

PTDXF was created to provide a secure alternative focused on visible information only.

---

## Does PTDXF replace PDF?

No.

PTDXF is designed to complement existing formats such as:

- PDF
- PDF/A
- DOCX
- ODT

PTDXF is intended for situations where security, auditability, and trusted document exchange are more important than advanced document functionality.

---

## What types of content can be stored in PTDXF?

PTDXF supports only:

- Pages
- Text
- Images

All content must be visible to the document reader.

---

## What content is prohibited?

PTDXF does not allow:

- Macros
- VBA
- JavaScript
- ActiveX
- Embedded files
- Audio
- Video
- Hyperlinks
- Forms
- Comments
- Change tracking
- Version history
- External resources
- Network references
- Executable content

---

## Why are hyperlinks removed?

Hyperlinks can be used for:

- Tracking
- Phishing
- Redirects
- External resource loading

To ensure trusted document exchange, PTDXF removes hyperlinks during export.

Only visible text remains.

Example:

Displayed text:

```text
Download Manual
```

Hidden hyperlink:

```text
https://example.com/download
```

Stored in PTDXF:

```text
Download Manual
```

---

## Why are macros not allowed?

Macros execute code.

Code execution inside document formats creates security risks and increases attack surface.

PTDXF prohibits all forms of executable document content.

---

## Why are embedded files prohibited?

Embedded files can be used to distribute:

- Malware
- Scripts
- Unauthorized content

PTDXF stores document information only.

Attachments are not part of the format.

---

## Does PTDXF support digital signatures?

Yes.

PTDXF may contain optional digital signatures used for:

- Authenticity verification
- Integrity verification
- Auditability

Digital signatures must not contain executable logic.

---

## Can PTDXF documents be searched?

Yes.

PTDXF supports full-text search.

Only visible information is searchable.

Removed or sanitized content is never searchable.

---

## How does PTDXF handle images?

PTDXF supports:

- JPEG
- PNG

During export:

- EXIF metadata is removed
- GPS information is removed
- Author information is removed
- Additional metadata is removed

All images must be displayed with a visible border.

---

## What are PTDXF Security Levels?

PTDXF defines three security levels.

### LEVEL 0 – Trusted

The document fully complies with the PTDXF specification.

Result:

```text
Document opened.
```

---

### LEVEL 1 – Sanitized

The document contains removable violations such as:

- Hyperlinks
- Metadata
- Comments

Result:

```text
Violations removed.
Document opened.
```

---

### LEVEL 2 – Critical Security Violation

The document contains:

- Unknown object types
- Structural manipulation
- Invalid binary blocks
- Integrity violations

Result:

```text
Document opening denied.
```

---

## What happens when a LEVEL 2 document is detected?

PTDXF refuses to display the document.

The user may optionally create a forensic text extraction.

Generated filename:

```text
<DocumentName>_(potentially_malicious).txt
```

The extracted file is intended for security professionals and forensic analysis.

---

## Why does PTDXF validate files when opening?

PTDXF follows a dual-protection approach:

1. Sanitize during creation.
2. Validate again during opening.

This helps detect manipulation occurring after document creation.

---

## Is PTDXF suitable for government use?

PTDXF was designed with the following environments in mind:

- Government agencies
- Public administration
- Critical infrastructure
- Regulated industries
- Compliance programs
- Security-sensitive organizations

---

## Is PTDXF suitable for ISO 27001 environments?

Yes.

PTDXF supports secure document handling by reducing attack surface and limiting document content to visible information.

PTDXF may support compliance requirements related to:

- Information protection
- Secure document exchange
- Auditability

Implementation-specific compliance assessments remain the responsibility of the deploying organization.

---

## Is PTDXF suitable for TISAX environments?

Yes.

PTDXF can support secure information exchange processes by removing active and hidden document content prior to document sharing.

PTDXF is intended to reduce risks associated with document-based attack vectors.

---

## Is PTDXF open source?

The PTDXF specification is intended to be publicly available.

Reference implementations may be released under open-source licenses.

Future certification programs and trademarks may be governed separately.

---

## Can software vendors implement PTDXF?

Yes.

The goal of PTDXF is interoperability.

Software vendors may implement PTDXF compatibility according to the public specification.

Certification marks may require additional verification.

---

## Does PTDXF support AI systems?

PTDXF is designed to be AI-friendly.

Optional image classifications may assist machine interpretation:

- photo
- technical_drawing
- electrical_schematic
- blueprint
- process_diagram
- flow_chart
- table_scan

These classifications describe only the document type and shall not contain hidden information.

---

## What is the core principle of PTDXF?

> What would not be visible on a printed document shall neither be stored nor displayed in a PTDXF document.

---

## Official Motto

**Visible Information. Nothing More.**

**What is not visible shall not exist.**
