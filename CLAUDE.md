# Orchestrated Diamond - TeXFlow Project

## Project Overview

This project converts "The Orchestrated Diamond: A Framework for Mixed-Initiative Co-Creation in Design" from DOCX to a professional academic LaTeX document using TeXFlow tools.

## TeXFlow Tool Usage

This project extensively uses **TeXFlow** - a comprehensive document management system for LaTeX workflows. TeXFlow provides specialized tools for:

### Document Management
- **Project Organization**: TeXFlow project structure with `content/`, `output/`, and `assets/` directories
- **Format Conversion**: DOCX → LaTeX → PDF conversion pipeline
- **Document Validation**: LaTeX syntax checking and compilation verification

### Bibliography Management  
- **BibTeX Integration**: 74 references converted from manual citations to proper BibTeX format
- **Citation System**: Numbered citations [1]-[48] with automatic bibliography generation
- **Reference Validation**: Ensures all citations are properly linked and formatted

### Academic Formatting
- **Professional Structure**: Title, author, abstract, sections, and bibliography
- **Citation Styles**: Numeric citation format with proper academic referencing
- **Typography**: Academic margins, spacing, and font selection

## Key TeXFlow Commands Used

```bash
# Project setup
mcp__texflow__project(action="import", name="the_orchestrated_diamond")

# Document conversion
mcp__texflow__document(action="convert", source="document.docx", target_format="latex")
mcp__texflow__document(action="convert", source="document.tex", target_format="pdf")

# Document editing
mcp__texflow__document(action="read", path="document.tex", window_start=X, window_size=Y)
mcp__texflow__document(action="edit", path="document.tex", old_string="...", new_string="...")

# PDF inspection
mcp__texflow__document(action="inspect", path="document.pdf", page=N)

# Document validation
mcp__texflow__document(action="validate", path="document.tex")
```

## Project Structure

- **`content/`**: Source files (DOCX, LaTeX, BibTeX)
- **`output/pdf/`**: Final compiled PDF documents
- **`references.bib`**: Complete bibliography database (74 entries)
- **LaTeX compilation**: Uses XeLaTeX + Biber for advanced typography and bibliography

## Author Information

**Aaron Bockelie**  
Independent Researcher, Wichita, Kansas

## Technical Notes

- **Bibliography System**: BibLaTeX with numeric style and Biber backend
- **Document Class**: KOMA-Script `scrartcl` for professional academic formatting  
- **Citation Count**: 48 active citations from 74 available references
- **Page Count**: 32 pages with complete structure and bibliography

This project demonstrates TeXFlow's capability to handle complex academic document conversion while maintaining professional formatting and complete bibliography management.