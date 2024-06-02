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

```{image} ../graphics/TripoliOpeningScreen.png
:alt: Tripoli Opening Screen
:align: center
```

# Start Tripoli

The easiest way to start Tripoli is to double-click on the Tripoli .jar file you downloaded.  However, depending on your computer's security settings, you might get hassled by some warnings.  Here's what to do:

## Mac:

The security settings on your Mac are likely configured so that you get a warning when you try and open an app that you downloaded from the internet.  Tripoli is not malware, and we are not secretly downloading your unpublished data -- we have enough of our own!  To open Tripoli anyway, open System Settings (the gear icon on your dock), then click on "✋ Privacy and Security" in the left-hand menu. Scroll down on the right-hand side of the window until you see a prompt asking if you want to "Open Anyway". 

```{image} ../graphics/MacPrivacyAndSecuritySettings.png
:alt: Mac Privacy and Security Settings
:width: 400px
:align: center
```

Click the "Open Anyway" button, enter your password if needed, and the Tripoli application will open.  

You only need to go to Privacy and Security settings once to open this .jar file.  Double-clicking on it in the future will just open Tripoli.  However, when you download a new version of Tripoli with a new version number and filename, you'll need to repeat the process.  Or, you can open Tripoli from the command line using the instructions in the [Starting Tripoli](../using_Tripoli/05-StartingTripoli.md "Starting Tripoli") section.

## PC:

Double-clicking the Tripoli .jar file should work on a PC right away, as long as you've installed Java.  However, if you have an old Java installation, Windows might try and fail to open Tripoli with your older version.  To fix this problem, we've created a .bat file, which you can download here:

- {download}`Tripoli.bat <../testData/Tripoli.bat>`

Move both the Tripoli .jar file you want to run and the .bat file to a new folder, then double-click on the .bat file to open Tripoli.

## Linux: 

If you're running Linux, you probably have the expertise to use the [command line interface to open Tripoli](../using_Tripoli/05-StartingTripoli.md "Starting Tripoli").

# Loading data files into Tripoli

The easiest way to open a mass spectrometer data file in Tripoli is to drag and drop it into the Tripoli window.  Other methods are detailed in [Loading Data](../using_Tripoli/06-LoadingData.md "Loading Data").

## Find your data file

Open Windows Explorer, Mac Finder, or your Linux file manager.  If you don't have a data file handy, try a file from the KU TIMS:

- {download}`Pb data file <../testData/GHR1 20200827-11 Pb-6590.xls>`
- {download}`U data file <../testData/GHR1 20200827-11 U run2-6591.xls>`

## Drag and Drop

Drag and drop the data file out of your file manager and into Tripoli.  If there's already a data file open in Tripoli, that's ok!  Tripoli will add the new file to your session.  Read more about sessions at [Loading Data](../using_Tripoli/06-LoadingData.md "Loading Data").

# Interactively Visualize Your Data

After you open a data file, you'll immediately see a window full of plots.  

```{image} ../graphics/ExampleTripoliPlots.png
:alt: Tripoli Example Plots
:width:
:align: center
```

Buttons along the top of the window and inside each time series plot control the display of your data.  Hover your cursor over a plot to see a tooltip with mouse button actions to zoom in/out, enter "sculpt" mode to perform data rejection, and more.  The summary statistics beside each plot update as you reject or restore data, as do the graphical summaries shown as shaded regions behind the data points.

# Manage Your Analysis

The Tripoli "Analysis Manager" window behind your plots now shows details about your loaded analysis.  

```{image} ../graphics/TripoliAnalysisManager.png
:alt: Tripoli AnalysisManager
:width:
:align: center
```

An interactive panel at the bottom of the window contains checkboxes for showing or hiding different measured isotope ratios or intensities.  At the bottom of the Analysis Manager, there are buttons to launch the plot window as well as to export the (U-Pb) data to ET_Redux and to the clipboard.

# Manage Your Session

You can load more than one mass spectrometer file into Tripoli at a time.  Close the plot window if it's open, and then drag another mass spectrometer data file onto the main Tripoli window.  The new file and plots should open immediately.

To see both anayses in your new session, go to the menu at the top of the Tripoli window and choose Session -> Manage Session.  

```{image} ../graphics/TripoliManageSessionMenuSelection.png
:alt: Tripoli Session Manager
:width:
:align: center
```

You can name your session, see a list of the analyses included in this session, and add notes.  To save the entire session, including the data, data rejection, and data visualization choices for all analyses, go to Session -> Save Session as... The resulting session file will have the .tripoli extension.  

# Recap

Now you're ready to load more mass spectrometry data files, examine the results, and export your data interpretations.  Tripoli is still under active development.  If you findn issues or bugs, go to the main Tripoli menu and find Help -> Contribute an Issue on GitHub.  If you have a question or want to start a discussion about new features to add, go to the main Tripoli menu and find Help -> Visit Tripoli Discussions on GitHub.  Note that both require a GitHub username and password (these are very handy!).

For more detailed information on starting Tripoli, loading data, and making plots, please see the next section of the manual, Using Tripoli.

# Read More:

::::{grid} 1 1 2 3

:::{card}
:header: [Starting Tripoli](../using_Tripoli/05-StartingTripoli.md "Starting Tripoli")
Get Tripoli started using Java, from your file broswer or the command line.
:::

:::{card}
:header: [Loading Data](../using_Tripoli/06-LoadingData.md "Loading Data")
Learn what kinds of mass spectrometer files Tripoli will load and what Tripoli can do with your data.
:::

:::{card}
:header: [Making Plots](../using_Tripoli/07-MakingPlots.md "Making Plots")
Navigate the plot window, including interactions like zooming and data rejection.
:::
::::