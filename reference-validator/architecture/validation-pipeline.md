# Validation Pipeline

## Stage 1

Container Validation

Verify:

- ZIP structure
- Required files
- Manifest

---

## Stage 2

Schema Validation

Verify:

- manifest.schema.json
- page.schema.json
- image.schema.json
- security.schema.json

---

## Stage 3

Object Validation

Allowed:

- Page
- Text
- Image

Unknown objects trigger LEVEL 2.

---

## Stage 4

Security Validation

Check:

- Hyperlinks
- Metadata
- Attachments
- Scripts

---

## Stage 5

Level Determination

Determine:

- LEVEL 0
- LEVEL 1
- LEVEL 2

---

## Stage 6

Reporting

Create validation report.
