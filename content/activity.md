---
layout: default
title: 'Activity'
nav_order: 12
---
Step 1: Copy past only this part of an xml into an oXygen file:
```xml

<?xml version="1.0" encoding="UTF-8"?>
<TEI xmlns="http://www.tei-c.org/ns/1.0" xml:lang="en">
    <teiHeader><fileDesc>
            <titleStmt><title>Oscar Wilde’s Libel Suit</title> </titleStmt>
            <publicationStmt> <p>1895</p></publicationStmt>
            <sourceDesc><p> https://chroniclingamerica.loc.gov/lccn/sn85058130/1895-04-04/ed-1/seq-2/</p></sourceDesc>
        </fileDesc>
    </teiHeader>
    <text>
        <body>

```
Step 2: This will solve our problem:
```xml
 <fileDesc>
            <titleStmt>
                <title>Bike Ride</title>
            </titleStmt>
            <publicationStmt>
                <p>not published</p>
            </publicationStmt>
            <sourceDesc>
                <p>D. Leesing</p>
            </sourceDesc>
        </fileDesc>
```
