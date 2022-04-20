---
layout: default
title: Ticket Delivery Options
has_children: true
nav_order: 2
---

## Pelican OneCallAccess System Ticket Formats
Use the matrix below to understand which test ticket format is best for your organization and the system you utilize. Select the appropriate test ticket file to test with your TMS or in-house system. If you manually print tickets you can also download the PDF format to see the new printable version of the ticket.


| Option       | Who is it for?    | E-Mail Subject/Body | Available Formats  |
|:-------------|:------------------|:-------------|:-------------|
| Email Option 1     | Members without a ticket management system who wish to view or print their tickets in an easily readable format. |  Ticket Number,  General Information  |PDF |
| Email Option 2     | Can be printed/read, but is intended for members who will be parsing data into a ticket management system and/or GIS.	   |  Ticket Number,  Contains All ticket data  |GIF, GML| 
| Email Option 3     | Intended for use with ticket management system and/or GIS	|  Ticket Number,  Contains All ticket data  	|GIF, GML, XML| 
| Webhook      | Intended for use with ticket management system and/or GIS  | N/A  | JSON | 
| Legacy       | This is a replica of the format previously used in Newtin. It remains as an option for those that would like to continue recieving their tickets in this truncated format. | Ticket Number,  Contains ticket data | Plain Text | 

### Examples
<a href="https://usanorth811.github.io/pelicancorp/assets/zip/Option1.zip" class="btn mr-4">Option 1</a> <a href="https://usanorth811.github.io/pelicancorp/assets/zip/Option2.zip" class="btn mr-4">Option 2</a> <a href="https://usanorth811.github.io/pelicancorp/assets/zip/Option3.zip" class="btn mr-4">Option 3</a>

<a href='/pelicancorp/ticket_delivery/webhook.html' class='btn'>Webhook</a>

## Glossary of Formats
### PDF
The easiest format to use for members who plan on either printing or viewing their tickets on-screen, the PDF is a file format designed to present documents consistently across multiple devices and platforms.

### GIF
GIF is a standard image format. The GIF attachment will be an image of the job-site polygon as drawn or described by the excavator

### GML
The Geography Markup Language (GML) is the XML grammar defined by the Open Geospatial Consortium (OGC) . It allows for the transmission of the digsite polygon as a spatial object rather than as a picture.

### XML
Extensible Markup Language (XML) is a markup language that defines a set of rules for encoding documents in a format that is both human-readable and machine-readable. It provides a simple standard for transmitting ticket data to be consumed by most ticket-management systems.

### JSON
JSON is an open standard file format and data interchange format that uses human-readable text to store and transmit data objects consisting of attribute–value pairs and arrays. It is a common data format with diverse uses in electronic data interchange, including that of web applications with servers.