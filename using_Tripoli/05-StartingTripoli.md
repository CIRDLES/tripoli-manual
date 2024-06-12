---
title: Running the Tripoli Application
subject: Using Tripoli
subtitle: 
short_title: Starting Tripoli
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

# Before you start

Before you start Tripoli, make sure that you have:
- [x] Downloaded and installed the correct Java application,
- [x] Downloaded the latest Tripoli .jar file from the GitHub repository, and
- [x] Moved the Tripoli.jar file to a dedicated folder on your hard drive, for instance a folder named "Tripoli" inside your "Documents" folder.

# The easy way: double-click a .jar file 

In most cases, the simplest way to start the Tripoli application is to double-click on the .jar file you downloaded from [the GitHub repository](https://github.com/CIRDLES/Tripoli "GitHub Repository").  The .jar file contains everything you need to open the application and start reviewing data.  This approach is likely the best when setting up Tripoli on a shared lab computer, where users with a variety of software comfort levels will be opening Tripoli.  If you just double-clicked the Tripoli .jar file and nothing happened, or you got a warning, see OS-specific troubleshooting below.

```{include} ../setup/99-MacSecuritySettings.md
```

## PC:

If you're using an older version of Java for other applications on your PC, then it's possible that this older version is associated with your .jar file extension.  

But that's ok!  

You can have many Java distributions on your computer at one time.  You can still run your other Java applications with the same Java distribution you've been using, and run Tripoli with the newer distribution of Java that includes JavaFX that you downloaded using the [Java Installation Instructions](../setup/01-Installation.md "Java Installation Instructions").  Think of these Java distributions like foreign language translators.  The older distribution translates your older Java code into computer-readable instructions and your newer distribution translates the Tripoli software into computer-readable instructions.  As long as your computer is using the correct translator the process will be seamless, and both translators (or as many as you wish) can be installed on your computer at the same time.  

Unfortunately, when you double-click on a .jar file, your operating system has to make a choice about which Java distribution to use.  To point your OS to the newer version of Java when you're opening Tripoli, we've created a batch (.bat) file that contains the correct instructions.

- {download}`Tripoli.bat <../testData/Tripoli.bat>`

Move both the Tripoli .jar file you want to run and the .bat file to a new folder, then double-click on the .bat file to open Tripoli.  When you want to update Tripoli, then delete the .jar file for your older version of Tripoli and copy the newer .jar file into the folder with the .bat file.  

If this seems like a pain in the neck, then you might be interested in running Tripoli from the command line.  It's quick and easy.  

# The better way: the command line

A command line interface is a place to type instructions (command lines) that your computer will follow.  The advantage here is that you can issue specific commands to your computer and get additional low-level output from the programs you run.  While most of us spend most of our time in our operating system's graphical user interface double-clicking on apps to run them, the dinosaurs among the Tripoli user base will recognize an old friend in the familiar DOS prompt from eons ago.

## Mac

To use the command line, first you'll need to find it.  On a Mac, open Spotlight and type "Terminal" to open the Terminal app.  In Linux, you can usually open your Terminal app with `Ctrl`-`Alt`-`T`.  

To the left of your cursor, you'll see the name of the folder in your file system that you now have open.  To see the name of the complete path to this folder, type `pwd`.  Type `ls` to see the contents of the folder.  Navigate to your folder containing your Tripoli .jar file using `cd` to change your directory.  

## Windows

To use the command line, first you'll need to find it.  In Windows, go to the Start menu, type CMD and hit `<Enter>` to bring up the Command Prompt.  

To the left of your cursor, you'll see the name of the folder in your file system that you now have open.  

```{image} ../graphics/CommandPromptBlank.png
:alt: Windows Command Prompt
:width:
:align: center
```

Now navigate to the folder containing your Tripoli .jar file using `cd` to change directory as needed.  

If you don't know how to do this, no problem! Open File Explorer and navigate to the folder containing your Tripoli.jar file.  
```{image} ../graphics/WindowsFileExplorer.png
:alt: Windows File Explorer
:width:
:align: center
```

Now put your cursor in address bar at the top of the File Explorer window (just like the address bar on your web browser), type `cmd` and hit `<Enter>`.  You now have a Windows command prompt open to your Tripoli folder.  
```{image} ../graphics/CommandPromptBlank.png
:alt: Windows Command Prompt open to the Tripoli folder
:width:
:align: center
```

To run Tripoli from the command prompt using Java, type
`java -jar Tripoli-X.X.X.jar` where X.X.X is the version number of Tripoli you're using.  For instance, to run Tripoli version 0.5.1, type `java -jar Tripoli-0.5.1.jar`:
```{image} ../graphics/CommandPromptWithJava.png
:alt: Windows Command Prompt with Java command
:width:
:align: center
```
Type `<Enter>` to run Tripoli.  You've done it!

