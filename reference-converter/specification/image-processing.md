# Image Processing

# PTDXF Image Handling

Images are converted into PTDXF compliant image objects.

---

## Supported Formats

- JPEG
- PNG

---

## Metadata Removal

The converter shall remove:

- EXIF
- GPS
- Camera Information
- Author Information
- ICC Profiles

---

## Border Requirement

All images shall be displayed with a visible border.

---

## AI Classification

Optional:

- photo
- technical_drawing
- electrical_schematic
- blueprint
- flow_chart
- process_diagram
- table_scan

---

## Purpose

Image classes support machine interpretation only.

They shall not contain hidden information.

---

## Security Principle

Images shall contain visual information only.
