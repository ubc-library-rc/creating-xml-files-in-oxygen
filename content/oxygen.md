---
layout: default
title: 'oXygen'
nav_order: 10
---
# oXygen


## **XML editors**
There are many XML editors out there, but oXygen is one of the standard ones. Think of it as the "word processor" of XML files.

You can access it via the remote labs at UBC
[https://remotelabs.ubc.ca/#heading_1021](https://remotelabs.ubc.ca/#heading_1021)

### **Advantage**
- Helps identify flaws
- Has readymade TEI documents lined up

## **Create your first XML file in Oxygen**
Open Oxygen and open “New Document”


## **Drop this faulty code into the editor**
Input
{: .label .label-green }
```sh

<?XML version="1.0" encoding="UTF-8"?>
<TEI XMLns="http://www.tei-c.org/ns/1.0" XML:lang="en">
    <teiHeader>
       omitted
    </teiHeader>
    <text>
        <body>
            <div type="essay">
                <head First Nations places in Vancouver </head>
                <p> Yesterday, on <date> value= "August 3"</date> I came across a landmark which reminded me of the presence of the first nations. </p>
                <p> I rode along the sea wall and came across the <placeName>Welcome Figure </placeName>.
                 </p>

        </body>
    </text>
</TEI>
```

## **Header**
Input
{: .label .label-green }
```sh

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
```
### **Time to encode this sample in oXygen**
[https://chroniclingamerica.loc.gov/lccn/sn85058130/1895-04-04/ed-1/seq-2/(https://chroniclingamerica.loc.gov/lccn/sn85058130/1895-04-04/ed-1/seq-2/)

### **Task #5**
  What tags do we identify, and what would the tags look like?

### **Solution Task #5**
* *1*{: .circle .circle-blue} `Title: The Salt Lake Herald`
* *2*{: .circle .circle-red} `Date: Thursday, April 4 1895`
* *3*{: .circle .circle-yellow} `Num page=Page 2`
* *4*{: .circle .circle-green} `Title: Oscar Wilde’s Libel Suit`
* *5*{: .circle .circle-purple} `Subtitle: One of the most peculiar cases ever heard`
* *6*{: .circle .circle-blue} `Body of Text`
* *7*{: .circle .circle-blue} `Paragraphs`

## **What would this look like in the element structure?**
Input
{: .label .label-green }
```sh
                <head>The Salt Lake Herald</head>
                <placeName>Salt Lake City</placeName>,
                <date> Thursday, April 04, 1895</date>
                <head>Oscar Wilde’s Libel Suit <lb/>
                    One of the most peculiar cases ever heard <lb/>
                    Love letters to a boy </head>

```


## **All that is missing is our root element and header**
Input
{: .label .label-green }
```sh
<?XML version="1.0" encoding="UTF-8"?>

<TEI XMLns="http://www.tei-c.org/ns/1.0" XML:lang="en">
    <teiHeader>
        <fileDesc>
            <titleStmt>
                <title>Oscar Wilde’s Libel Suit</title>
            </titleStmt>
            <publicationStmt>
                <p>1895</p>
            </publicationStmt>
            <sourceDesc>
                <p> https://chroniclingamerica.loc.gov/lccn/sn85058130/1895-04-04/ed-1/seq-2/</p>
            </sourceDesc>
        </fileDesc>

    </teiHeader>


    <text>
        <body>
   ```
## **...and let's not forget the closing tags at the end of the document**

Input
{: .label .label-green }
```sh

        </body>
    </text>
    </TEI>

```
### **Additional Solution Task #5**

  Help: fill in the information into the gaps!
  [https://github.com/ubc-library-rc/creating-XML-files-in-oxygen/blob/main/Helper%20Oscar.XML](https://github.com/ubc-library-rc/creating-XML-files-in-oxygen/blob/main/Helper%20Oscar.XML)

  Complete solution:
  [https://github.com/ubc-library-rc/creating-XML-files-in-oxygen/blob/main/OSCAR.XML](https://github.com/ubc-library-rc/creating-XML-files-in-oxygen/blob/main/OSCAR.XML)

Congratulations!  You successfully created your first XML file!
There are so many more things to explore about XML and text encoding. Get inspired in the "Resources" Section!
