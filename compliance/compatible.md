# PTDXF Compatible

# Certification Level

PTDXF Compatible is the entry-level implementation category within the PTDXF ecosystem.

A PTDXF Compatible implementation demonstrates the ability to recognize and process PTDXF documents according to the public specification.

---

# Purpose

The purpose of PTDXF Compatible certification is to establish a minimum interoperability baseline between implementations.

Compatible implementations are able to:

- Open PTDXF documents
- Read PTDXF container structures
- Parse PTDXF object definitions
- Interpret PTDXF manifests

---

# Requirements

A PTDXF Compatible implementation shall:

### C-001

Recognize PTDXF files.

Supported extension:

```text
.ptdxf
```

---

### C-002

Read the PTDXF container structure.

---

### C-003

Parse:

- manifest.json
- page definitions
- text objects
- image objects

---

### C-004

Reject unsupported PTDXF versions.

---

### C-005

Display version information.

---

# Not Required

PTDXF Compatible implementations are not required to:

- Validate security levels
- Perform sanitization
- Execute compliance checks
- Support forensic extraction

---

# Intended Audience

Examples:

- Basic viewers
- Third-party integrations
- Development tools
- Prototype implementations

---

# Result

A PTDXF Compatible implementation provides basic interoperability but does not guarantee full specification compliance.

---

# Certification Mark

Eligible designation:

PTDXF Compatible
