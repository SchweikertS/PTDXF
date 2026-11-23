# PTDXF Converter Architecture

# Overview

The PTDXF Converter transforms existing document formats into compliant PTDXF documents.

The conversion process follows a strict security pipeline.

The objective is not document reproduction alone.

The objective is trusted document transformation and sanitization.

---

# Core Workflow

Input Document

↓

Import

↓

Extract Visible Content

↓

Sanitize Content

↓

Generate PTDXF

↓

Validate PTDXF

↓

Output PTDXF

---

# Design Principles

## Principle 1

Preserve visible information.

---

## Principle 2

Remove prohibited content.

---

## Principle 3

Reduce attack surface.

---

## Principle 4

Generate predictable output.

---

## Principle 5

Always produce specification-compliant PTDXF.

---

# Converter Components

## Importer

Reads source document.

Examples:

- PDF
- DOCX
- PPTX

---

## Extractor

Extracts:

- Text
- Images
- Page Structure

---

## Sanitizer

Removes:

- Hyperlinks
- Metadata
- Comments
- Scripts
- Macros
- Attachments

---

## Generator

Creates:

- manifest.json
- page objects
- text objects
- image objects
- security information

---

## Validator

Validates generated PTDXF.

Checks:

- Structure
- Object types
- Security rules

---

# Output

The generated PTDXF shall be:

- Valid
- Portable
- Secure
- Searchable
- Auditable
