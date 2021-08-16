---
layout: default
title: 'xml anatomy'
nav_order: 9
---
# Anatomy

Let's look at the details of what happens in a xml file. 
**Possible tags in a text document**

It all relies on identifiers: whether it is a line, a place or an author: we want to annotate (encode!) what information can be of interest in the respective file. 

Formalization
## **An xml document needs a neat form: Formalization**
Think of the Russian Matryoshka dolls: they need a top and a bottom part in order to function. That's how we make sure information is contained in the right place under the right tag. 


## **XML Anatomy**
This image will make more sense in 5 minutes. Look at the opening and closing tag! Just like the Matryoshka doll, they open and close the information we encoded.
Placeholder>IMAGE

## **Formalization: Box it!**
In the image, the  pink line delineates the document with the opening tag <div> and closing tag </div>
The value type=”act” specifies the genre! 
This is what we call the commandline or element.
<div type=”act”>
</div>

Placeholder>IMAGE

### **Task #2**
What other opening and closing tags can you identify comparing the scan of the manuscrupt and the xml code? Focus on the circled information -- we'll get to those other tags in a bit! 


### **Solutions**
Input
{: .label .label-green }
```sh
<head> </head>
  <stage> </stage>
    <speaker> </speaker>
      <div> </div>
      <p> </p>

```




### **Task #3**
What tags would you want to single out in this newspaper clipping?
Placeholder>IMAGE


### **Solutions**
Input
{: .label .label-green }
```sh
<name>UNIVERSITY OF VIRGINIA, CHARLOTTESVILLE</name> 
<num>NUMBER 92</num>
<head>THE CAVALIER DAILY</head>
<date>TUESDAY, MARCH 11, 1969</date>

etc. 
```
## **Attributes**
Input
{: .label .label-green }
```sh

<div1 type="nameplate">

<head>THE CAVALIER DAILY</head>
<ab><name type="place">UNIVERSITY OF VIRGINIA, CHARLOTTESVILLE</name>, 
<date value="1969-03-11">TUESDAY, MARCH 11, 1969</date> 
<num type="number" value="92">NUMBER 92</num></ab>
</div1>
```
The attribute name specifies the tag. Its matching value and type follows the = sign and is marked by “”

## **Divisions**
Input
{: .label .label-green }
```sh

Big chunks
<div> big divisions
<head> 
<ab> anonymous block
Mid size
<p> paraphraphs
Small pieces
<title> 
<head>
<l>
```
 
## **A well-formed xml file**
It specifies which source and thereby data set it orients with one root element 
 Input
{: .label .label-green }
```sh
<TEI xmlns:html="http://www.w3.org/1999/xhtml"
     xmlns="http://www.tei-c.org/ns/1.0" >
```
  
It has a header
  Input
{: .label .label-green }
```sh
<teiHeader> 
 	<fileDesc>
            <titleStmt>
                <title>Bike Ride</title>
            </titleStmt>
            <publicationStmt>
                <p>not published</p>
            </publicationStmt>
            <sourceDesc>
                <p>D.Leesing</p>
            </sourceDesc>
        </fileDesc>
  </teiHeader> 

</TEI>

```
Comparable quoting and signatures " … "
It is always symmetric <> </>
  

## **A valid xml file**
Plays by the rule book (depending which markup rule book is used (e.g. TEI, xhtml (turning it into a webpage))

### **Task #4**
Find the lemons! (validity)

Placeholder> IMAGE1
Placeholder> IMAGE2
Placeholder> IMAGE3



