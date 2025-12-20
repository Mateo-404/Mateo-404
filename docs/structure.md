# Repository Structure Overview

This repository is organized to clearly separate **presentation**, **data**, and **documentation**, following common software engineering best practices.

## Root

- `README.md`  
  Public GitHub profile README.  
  Contains a concise, curated presentation (about me, stack, links).  
  It is **not** the source of truth for the CV.

## Data

- `data/cv.json`  
  Curriculum Vitae in **JSON Resume** format.  
  This is the **structured source of truth** for professional information.  
  Designed to be reusable by tools, websites, or automated processes.

## Documentation

- `docs/cv.md`  
  Documentation explaining the purpose, format, and usage of `cv.json`.  
  Includes references to external viewers and the public PDF CV.

## Design Principles

- **Separation of concerns**  
  - README → presentation  
  - JSON → data  
  - docs → explanation

- **No duplication**  
  The same information is not maintained in multiple formats.

- **Scalability**  
  The structure allows future additions (scripts, generators, exports) without refactoring.

## External References

- PDF CV and portfolio are hosted externally to avoid duplication and desynchronization.
