---
title: Getting Started in Tripoli
subject: Setup
subtitle: 
short_title: Quick Start
authors:
  - name: Noah McLean
    affiliation:
      - University of Kansas
    orcid: 0000-0003-0388-1862
    email: noahmc@ku.edu
license: CC-BY-4.0
keywords: 
exports:
  - format: docx
  - format: pdf
    template: eartharxiv
    article_type: Report
numbering:
  code: false
  headings: true
---

# Start Tripoli

The easiest way to start Tripoli is to double-click on the Tripoli .jar file you downloaded.  However, depending on your computer's security settings, you might get hassled by some warnings.  Here's what to do:

## Mac:

The security settings on your Mac are likely configured so that you get a warning when you try and open an app that you downloaded from the internet.  Tripoli is not malware, and we are not secretly downloading your unpublished data -- we have enough of our own!  To open Tripoli anyway, open System Settings (the gear icon on your dock), then click on "✋ Privacy and Security" in the left-hand menu. Scroll down on the right-hand side of the window until you see a prompt asking if you want to "Open  Anyway". 

```{image} ../graphics/MacPrivacyAndSecuritySettings.png
:alt: Mac Privacy and Security Settings
:width: 400px
:align: center
```

Click the "Open Anyway" button, enter your password if needed, and the Tripoli application will open.  

You only need to go to Privacy and Security settings once to open this .jar file.  Double-clicking on it in the future will just open Tripoli.  However, when you download a new version of Tripoli with a new version number and filename, you'll need to repeat the process.  Or, you can 

## PC:

Double-clicking the Tripoli .jar file should work on a PC right away, as long as you've installed Java.  However, if you have an old Java installation, Windows might try and fail to open Tripoli with your older version.  To fix this problem, we've created a .bat file, downloadable from GitHub in 'Assets' right beside the .jar file.  Download both, then double-click the .bat file to open Tripoli.

## Linux: 

If you're running Linux, you might be interested in 

# Loading data files into Tripoli

The easiest way to open a mass spectrometer data file in Tripoli is to drag and drop it into the Tripoli window.  Other methods are detailed in [Loading Data](../using_Tripoli/06-LoadingData.md "Loading Data").

## Find your data file

Open Windows Explorer, Mac Finder, or your Linux file manager.  If you don't have a data file handy, try a file from the KU TIMS:

- {download}`Pb data file <../testData/GHR1 20200827-11 Pb-6590.xls>`
- {download}`U data file <../testData/GHR1 20200827-11 U run2-6591.xls>`

## Drag and Drop

Drag and drop the data file out of your file manager and into Tripoli.  If there's already a data file open in Tripoli, that's ok!  Tripoli will add the new file to your session.  Read more about sessions at [Loading Data](../using_Tripoli/06-LoadingData.md "Loading Data").

# Interactively Visualize your Data

After you open a data file, you'll immediately see a window full of plots.  