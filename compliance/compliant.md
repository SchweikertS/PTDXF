# PTDXF Compliant

# Certification Level

PTDXF Compliant is the standard implementation level for software that fully supports the PTDXF specification.

A PTDXF Compliant implementation shall support document validation, security level determination, and specification enforcement.

---

# Purpose

The purpose of PTDXF Compliant certification is to ensure that implementations correctly enforce PTDXF security and compliance requirements.

A compliant implementation shall be capable of identifying non-conforming content and reacting according to the specification.

---

# Requirements

## CO-001

All PTDXF Compatible requirements shall be fulfilled.

---

## CO-002

The implementation shall validate PTDXF document structures.

Validation shall include:

- Container structure
- Manifest structure
- Page structures
- Text objects
- Image objects

---

## CO-003

The implementation shall support PTDXF Security Levels.

Required:

- LEVEL 0
- LEVEL 1
- LEVEL 2

---

## CO-004

The implementation shall support PTDXF Validation Rules.

Validation shall include, but is not limited to:

- Allowed object types
- Allowed image formats
- Forbidden content checks
- Structural verification
- Integrity verification

---

## CO-005

The implementation shall detect prohibited content.

Prohibited content includes:

- Hyperlinks
- Scripts
- Embedded files
- Forms
- External resources
- Active content

---

## CO-006

The implementation shall enforce LEVEL 1 processing.

Removable violations shall be:

- Identified
- Removed
- Reported

Examples:

- Hyperlinks
- Metadata
- Comments

---

## CO-007

The implementation shall enforce LEVEL 2 processing.

When violations cannot be safely removed:

- Document opening shall be denied
- Document display shall be denied

Examples:

- Unknown object types
- Structural manipulation
- Invalid binary sections
- Integrity violations

---

## CO-008

The implementation shall create validation results.

Minimum information:

- Validation timestamp
- Security level
- Detected violations
- Performed actions

---

## CO-009

The implementation shall support audit logging.

Validation activities shall be traceable.

---

## CO-010

The implementation shall support full-text search on visible text content.

Removed or rejected content shall not be searchable.

---

# Security Level Requirements

---

## LEVEL 0

Conditions:

- Fully compliant document
- No violations

Action:

- Open
- Display
- Search
- Print

---

## LEVEL 1

Conditions:

- Removable violations detected

Action:

- Sanitize
- Revalidate
- Display sanitized version

The original non-compliant content shall not be displayed.

---

## LEVEL 2

Conditions:

- Critical violations detected

Action:

- Reject document
- Deny display

Optional:

- Offer forensic extraction

---

# Reporting Requirements

Validation reports shall include:

- Document name
- Validation date
- Validation result
- Security level
- Violations detected
- Actions performed

---

# Conformance Statement

A PTDXF Compliant implementation shall enforce the PTDXF specification and shall not silently ignore specification violations.

Unknown structures shall be treated as violations.

---

# Certification Mark

Eligible designation:

PTDXF Compliant

---

# Purpose of Compliance

PTDXF Compliant implementations provide a predictable and auditable foundation for:

- Trusted document exchange
- Compliance workflows
- Security-sensitive environments
- Government use
- Long-term archiving

while maintaining interoperability with the PTDXF ecosystem.
