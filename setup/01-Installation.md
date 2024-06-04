---
title: Java Download and Installation
subject: Setup
subtitle: for Tripoli Users
short_title: Install Java
date: May 13, 2024
affiliations:
    - id: KU
      institution: University of Kansas
      department: Department of Geology
      city: Lawrence
      region: Kansas
authors:
  - name: Noah McLean
    affiliation: KU
    orcid: 0000-0003-0388-1862
    email: noahmc@ku.edu
license: CC-BY-4.0
# keywords: documentation, myst
exports:
  - format: docx
  - format: pdf
    id: paper
    template: lapreprint-typst
numbering:
  code: false
  headings: true
---

Before running Tripoli, you need to download [Java](wiki:Java_(software_platform)) and install it on your computer.  Tripoli is written in the programming language Java, and it runs on your computer (Windows, Mac, or Linux) using the Java platform.  Because it is open source, you can download the latest version of Java for free from several reputable distributors, including Liberica and Azul.  You can pick your distribution as long as it includes JavaFX, which has support for rich graphics, and the version is 17 or higher. The following have been tested and work with Tripoli.  

# Gather some information about your computer

You've probably needed this information before to install software on your computer.  You should know:
1. Your operating system: Linux, Mac, or Windows, 
2. Whether you have a 64-bit (probably) or a 32-bit processor (much older)
3. Does your processor use the x86 or ARM architecture?  

Newer Apple products use Apple Silicon (e.g., the M1, M2, etc chips) with an ARM architecture, and older Apple products with Intel chips and Windows machines usually use an x86-compatible architecture.  For more information, google how to determine what type of processor is in your computer, then whether it is x86 or ARM.  

# Download a Java Distribution

## Liberica Distribution (Choice 1, easier install)
1. Go to the bellsoft Liberica page [here](https://bell-sw.com/pages/downloads/#jdk-21-lts "bellsoft Liberica downloads").  
2. Scroll down past the banners the until you the list of 64-bit operating systems and options.  If you have a 32-bit operating system, scroll down just a little farther.
```{image} ../graphics/Liberica_OS_Options.png
:alt: Liberica OS Options
:width: 400px
:align: left
```
3. Underneath the name of your operating system, choose your processor architecture (x86 or ARM), then click on the dropdown menu and choose "Package: Full JRE".  For instance, on a Mac with an Intel processor, your choice would look like this, though version numbers are frequently updated:
```{image} ../graphics/Liberica_macOS_FullJRE.png
:alt: macOS Full JRE
:width: 600px
:align: left
```
4. Click on the blue text link to the right corresponding to your favorite installer type.  For a Mac, DMG and for Windows, MSI are easy to use.
5. Once downloaded, run the installer, click through the prompts, and type in your password as needed.  Congratulations, you've installed Java!  

## Azul Distribution (Choice 2, more complicated)
1. Go to the Azul distribution page [here](https://www.azul.com/downloads/?version=java-21-lts&package=jre-fx#zulu "Azul Java Distributions").  This page should show you only downloads for Java 21 (LTS means long-term stable) and JRE packages (Java Runtime Environment -- what you need to run Java on your computer).
2. In the set of dropdown menus at the top, choose your operating system and architecture.  Alternately, find your operating system and architecture in the list below the dropdown menus.  
```{image} ../graphics/Azul_OS_Options.png
:alt: Azul OS Options
:width: 500px
:align: left
```
3. Hover your cursor over the dark blue Download button next to your OS and architecture, then choose a download file type.  For Mac and Windows, a .zip file is good.
4. Your download will start and a bunch of advertisements and some pop-ups will show up.  Ignore them and find the .zip file in your browser or computer's Downloads folder.
5. Copy the .zip file to a dedicated folder on your hard drive, then unzip the folder and delete the .zip archive.
6. Add the installation folder to your `PATH` environment variable. Don't know how to do this? Google will help for your system, or just use Liberica (Choice 1).
7. Congratulations, you've installed Java!
