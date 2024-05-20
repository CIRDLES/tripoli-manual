---
title: Tripoli
exports:
  - format: pdf
    template: plain_latex_book
    output: exports/tripoli-manual.pdf
    toc: _toc.yml
---
```{image} graphics/TripoliLogoLarge.png
:alt: Tripoli Logo
:width: 200px
:align: center
```

Tripoli is free, open-source software to visualize, interpret, and reduce mass spectrometer data from thermal ionization and multi-collector ICP mass spectrometers.  Load mass spectrometer files into Tripoli, get interactive visualizations, and produce a variety of output formats that fit into your workflow.  

Tripoli was developed with a [grant](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2149084 "NSF Award Details") from the National Science Foundation to Noah McLean, Jim Bowring, and Scott Burdick, and has benefitted greatly from contributions by members of [CIRDLES](https://cirdles.org/ "CIRDLES") and the isotope geochemistry and geochronology community.

The current Tripoli project is built on a previous program with the same name.  The original version of Tripoli, which we now call "OG Tripoli" was Windows- and TIMS-only.  We're reproducing and expanding on OG Tripoli's capabilities with this project, but you can find more info about OG Tripoli [here](https://cirdles.org/projects/tripoli/ "OG Tripoli").


## Supported Operating Systems

Tripoli runs in Java and therefore works on Windows, Mac, and Linux operating systems.  You will need to [install Java before running Tripoli](./01-Installation.md).  


## Supported Mass Spectrometers

Tripoli supports import of file formats from the following mass spectrometers.  Don't see your instrument or file format?  Contact us [here](https://github.com/CIRDLES/Tripoli/issues/new "Tripoli GitHub Issues").  

**Current, TIMS:**
- Isotopx Phoenix (IonVantage .xls, Isolinx .timsdp)
- Nu TIMS (Individual Answers .txt)
- Thermo Triton (.exp)

**Planned, MC-ICPMS:**
- Nu Plasma 3
- Thermo Neptune (±Plus)


## Getting Started with Tripoli

Brand new to Tripoli? Get started here:
1. [Install Java](./01-Installation.md)
2. [Download Tripoli](./02-InstallTripoli.md)
3. [Quick Start](./03-QuickStart.md)
