---
layout: default
title: 'Application'
nav_order: 7
---

Let's first understand what scope and presets a project has before we dive into how to create xml files. 

Here, we want to understand 

* *1*{: .circle .circle-blue} `Sources`
* *2*{: .circle .circle-red} `Application`

This example uses poems written by the excentric German-American writer Baroness Elsa von Freytag-Loringhoven. What a woman, check her out after this course!
https://digital.lib.umd.edu/transition/index.html

As a source, the project created by Tanya Clement in 2008 takes the .tiff scans of the original, handwritten poem and compares it to a reworked second version of the poem. 

As an application, the encoded transcriptions make it possible to compare e.g. line changes. 

**Task #1**

Assess the following examples and think about:

1) What are the sources/texts used in the project?
2) What is the main function in the project? 

Please choose any of these three text encoding projects!

A) Wilde Trials International News Archive https://dhil.lib.sfu.ca/wilde/index.html

B) The Colonial Despatches 
https://bcgenesis.uvic.ca/index.html

C) Map of London
https://mapoflondon.uvic.ca/


**Solutions**
A)
Wilde Trials International News Archive 
https://dhil.lib.sfu.ca/wilde/index.html

Source: Newspaper transcriptions in various languages of the Wilde trials
Function: Compare similarities in either language, search transcriptions

B)
Application / Colonial Despatches
https://bcgenesis.uvic.ca/index.html
Source: “original correspondence between the British Colonial Office and the colonies of Vancouver Island and British Columbia. images have been generated from monochrome microfilms”
transcriptions
Function: “Direct comparison between scanned image and transcription”

C) 
Application / Map of London
https://mapoflondon.uvic.ca/
Source: “Civitas Londinum is a bird’s-eye view of London first printed from woodblocks in about 1561” 
Function: Identify landmarks, find ressources for the landmark, (contribute to the map)

**Where’s the xml in these projects?!**

Let’s look at the xml files in one of the respective projects! 
http://v-machine.org/samples/orchardFarming.xml

Display of xml

![Machine](http://github.com/ubc-library-rc/creating-xml-files-in-oxygen/blob/main/content/images/Versioning%20machine%20Orchard.png)

Xml file
![xml file](http://github.com/ubc-library-rc/creating-xml-files-in-oxygen/blob/main/content/images/xml%20Orchard.png)


**xml vs html**
xml is a language which stores texts and categorizes the information, it does not “do” anything on its own. 
It is an eXtensible Markup Language (XML) - that means that it is your choice what to tag - and you can define it!


html is a programming language which can be used in order to display information (e.g. how a website is structured, what it looks like, etc.)


A processing application, written in html or javascript is necessary in order to display our xml documents.

**Processing application: Versioning Machine**

Two parts are necessary to convert text:

We need 1)encoded xml files and we need 2) a processing application which reads and displays the xml files in a certain way. 
One example is “The Versioning Machine 5.0”

http://v-machine.org/




