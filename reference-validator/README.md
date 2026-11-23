# PTDXF Reference Validator

The PTDXF Reference Validator is the official validation implementation for PTDXF documents.

Its purpose is to determine whether a document complies with the PTDXF specification and to assign an appropriate security level.

---

## Functions

The validator shall:

- Verify document structure
- Validate object types
- Detect prohibited content
- Determine security level
- Generate validation reports
- Support forensic extraction for LEVEL 2 documents

---

## Security Levels

### LEVEL 0

Trusted

Document fully complies with PTDXF.

---

### LEVEL 1

Sanitized

Removable violations detected.

---

### LEVEL 2

Critical Security Violation

Document rejected.

---

## Output

Examples:

```text
LEVEL 0
Document Valid
```

```text
LEVEL 1
2 Hyperlinks Removed
Document Sanitized
```

```text
LEVEL 2
Unknown Object Type Detected
Document Rejected
```
