# AI Support

# PTDXF and Artificial Intelligence

PTDXF is designed to simplify machine interpretation of document content.

---

## Why AI Support Matters

Many modern document formats were created for visual presentation rather than machine understanding.

Common challenges include:

- Complex layouts
- Ambiguous reading order
- Embedded content
- Hidden structures

PTDXF reduces these challenges.

---

## Simple Document Structure

PTDXF supports only:

- Pages
- Text
- Images

This results in a predictable structure for AI systems.

---

## Reading Order

PTDXF stores content in logical reading order whenever possible.

This improves:

- Text extraction
- Summarization
- Search
- Classification

---

## Image Classification

PTDXF allows optional image class declarations.

Examples:

```text
photo
technical_drawing
electrical_schematic
blueprint
process_diagram
flow_chart
table_scan
```

---

## Purpose

Image classes help AI systems understand what type of image they are processing.

Example:

```text
technical_drawing
```

The image remains unchanged.

The classification simply informs the AI about the expected content type.

---

## Technical Drawings

Potential AI applications:

- Drawing classification
- Dimension extraction
- Revision identification
- Component detection

---

## Electrical Schematics

Potential AI applications:

- Symbol recognition
- Connection analysis
- Component indexing
- Documentation support

---

## No Hidden AI Metadata

PTDXF intentionally avoids storing:

- AI-generated descriptions
- AI-generated summaries
- AI-generated interpretations

Reason:

PTDXF stores visible information only.

---

## AI Principle

AI support must not introduce hidden information.

Machine-readable classification is allowed.

Machine-generated content storage is not.

---

## Conclusion

PTDXF aims to provide a clean and predictable foundation for future AI-supported document processing while preserving transparency and auditability.
