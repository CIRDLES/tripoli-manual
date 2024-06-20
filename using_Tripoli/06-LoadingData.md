---
title: Loading Data Into Tripoli
subject: Manual
subtitle: 
date: 6/20/2024
short_title: Loading Data
authors:
  - name: Noah McLean
    affiliation:
      - University of Kansas
    orcid: 0000-0003-0388-1862
    email: noahmc@ku.edu
license: CC-BY-4.0
keywords: documentation
exports:
  - format: docx
  - format: pdf
    template: eartharxiv
    article_type: Report
numbering:
  code: false
  headings: true
---

(supportedFileTypes)=
# Supported file types

You can currently load data into Tripoli from the following mass spectrometer data files:

**Current, TIMS:**
- Isotopx Phoenix (IonVantage .xls, Isolinx .timsdp)
- Nu TIMS (Individual Answers .txt)
- Thermo Triton (.exp)

**Planned, MC-ICPMS:**
- Thermo Neptune ±Plus (in progress)
- Nu Plasma 3

# Ways to open files and load data

There are two ways to open a data file in Tripoli, described in separate sections below.

1. [Drag and drop a file](#dragAndDrop) from your file manager (e.g., File Explorer or Finder) directly into Tripoli.
2. Use [the load button](#loadButton) from the Analysis window.


(dragAndDrop)=
## Drag and drop

Locate the mass spectrometer file in your file manager, like Windows Explorer on a PC or Finder on a Mac.  Make sure that your have found the right file type, and not a folder of data and method files.  See [Supported file types](#supported-file-types) for the types of files Tripoli currently opens.  

You can drag and drop your mass spectrometer data file (left click and drag) into the blank Tripoli opening screen (with the Tripoli logo on a mango sorbet color gradient).  This will automatically open the file and open a window containing plots of all your measured data by default.

If you already have one analysis open, you can drag and drop another right onto the open Analysis window.  This action adds your second analysis to the same session as your first analysis.  For more details, see LINK TO SESSIONS AND ANALYSES.

(loadButton)=
## The Load Button 

Before you load a data file with the load button, you'll need to make a new Analysis.  An analysis contains your mass spectrometer data, plus some extra information about the data.  

```{image} ../graphics/NewAnalysisMenuSelected.png
:alt: Create a new analysis from menu option
:align: center
```

