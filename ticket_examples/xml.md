---
layout: default
title: XML
parent: Ticket Examples
nav_order: 4
---

## XML
Extensible Markup Language (XML) is a markup language that defines a set of rules for encoding documents in a format that is both human-readable and machine-readable. It provides a simple standard for transmitting ticket data to be consumed by most ticket-management systems.

<small>*The fields for "Anticipated Depth" and "Work Duration" are only being used in California and will remain blank on all Nevada tickets.</small>

<a href="https://usanorth811.org/images/USNCA-ONE-ANA-USA-North-811-Northern-California-TT55923-OneCallAccess-Webhook-Member-Guide.pdf" class="btn mr-4">California</a>
<a href="https://usanorth811.org/images/USNNV-ONE-ANA-USA-North-811-Nevada-TT55923-OneCallAccess-Webhook-Member-Guide.pdf" class="btn mr-4">Nevada</a>

```xml
<?xml version="1.0" encoding="utf-8"?>
<onecall:OneCallReferral xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:onecall="http://www.pelicancorp.com/onecall" xsi:schemaLocation="https://www.pelicancorp.com/onecall/usan.xsd">
  <onecall:ReferralDetails>
    <onecall:MessageVersionNumber>1.0.10</onecall:MessageVersionNumber>
    <onecall:From>USA NORTH 811</onecall:From>
    <onecall:TicketMedium>Web</onecall:TicketMedium>
    <onecall:UtilityID>10504</onecall:UtilityID>
    <onecall:StationCode>CNSA12</onecall:StationCode>
    <onecall:UtilityName>California North State Authority</onecall:UtilityName>
    <onecall:To>Mark Scopece</onecall:To>
    <onecall:JobNumber>11</onecall:JobNumber>
    <onecall:TicketNumber>2022041100005</onecall:TicketNumber>
    <onecall:TicketRevisionNumber>000</onecall:TicketRevisionNumber>
    <onecall:PreviousTicketNumber xsi:nil="true"/>
    <onecall:PreviousTicketRevNumber xsi:nil="true"/>
    <onecall:SequenceNumber>4</onecall:SequenceNumber>
    <onecall:TransmissionID>123456789012</onecall:TransmissionID>
    <onecall:SubmittedDate>2022-04-11T11:13:39.018116-07:00</onecall:SubmittedDate>
    <onecall:WorkBeginDate>2022-04-11T11:12:00-07:00</onecall:WorkBeginDate>
    <onecall:LegalStartDate>2022-04-13T11:13:39-07:00</onecall:LegalStartDate>
    <onecall:TicketExpirationDate>2022-05-09T23:59:59-07:00</onecall:TicketExpirationDate>
    <onecall:WorkDuration>2-4 Days</onecall:WorkDuration>
	<onecall:IsEmergency>false</onecall:IsEmergency>
    <onecall:TicketStatus>Original</onecall:TicketStatus>
    <onecall:TicketType>Short Notice</onecall:TicketType>
    <onecall:WorkType>Environmental</onecall:WorkType>
    <onecall:WorkActivity>Fuel Tank(s) Work</onecall:WorkActivity>
    <onecall:DelineatedMethod>No</onecall:DelineatedMethod>
	<onecall:ExcavationSize>105891 Sq Ft</onecall:ExcavationSize>
    <onecall:ExcavationMethod>Boring - vertical</onecall:ExcavationMethod>
    <onecall:VacuumExcavation>true</onecall:VacuumExcavation>
    <onecall:AnticipatedDepth>&gt;84 inches</onecall:AnticipatedDepth>
    <onecall:ResponseRequired>true</onecall:ResponseRequired>
    <onecall:ProjectOwner>Fresno County</onecall:ProjectOwner>
    <onecall:Permit>County 12345678901234567890</onecall:Permit>
    <onecall:JobNoName xsi:nil="true"/>
    <onecall:StationList>
      <onecall:StationCode>CNSA12</onecall:StationCode>
    </onecall:StationList>
  </onecall:ReferralDetails>
  <onecall:CustomerDetails>
    <onecall:ExcavatorID>25</onecall:ExcavatorID>
    <onecall:Name>Martine Savary</onecall:Name>
    <onecall:Company>--Not Listed--</onecall:Company>
    <onecall:StreetAddress>123</onecall:StreetAddress>
    <onecall:CityTownPlace>Clovis</onecall:CityTownPlace>
    <onecall:State>CA</onecall:State>
    <onecall:Zipcode>33564</onecall:Zipcode>
    <onecall:UserType>Agriculture</onecall:UserType>
	<onecall:UserIndustry>Homeowner</onecall:UserIndustry>
    <onecall:Phone>541-565-6565</onecall:Phone>
    <onecall:Mobile xsi:nil="true"/>
    <onecall:Email>martine.savary@pelicancorp.com</onecall:Email>
    <onecall:Language>English</onecall:Language>
  </onecall:CustomerDetails>
  <onecall:LocationDetails>
    <onecall:AddressLocation>1055 Fowler Ave</onecall:AddressLocation>
    <onecall:CityTownPlace>Clovis</onecall:CityTownPlace>
    <onecall:County>Fresno</onecall:County>
    <onecall:State>CA</onecall:State>
    <onecall:NearbyCrossStreet>Barstow ave</onecall:NearbyCrossStreet>
    <onecall:StreetSidewalk>true</onecall:StreetSidewalk>
    <onecall:SubdivisionLot xsi:nil="true"/>
    <onecall:OnsiteContactName>Martine</onecall:OnsiteContactName>
    <onecall:OnsiteContactPhone>4189484444</onecall:OnsiteContactPhone>
    <onecall:Latitude>36.817805</onecall:Latitude>
    <onecall:Longitude>-119.681675</onecall:Longitude>
    <onecall:ExcavatorRemarks>test ticket</onecall:ExcavatorRemarks>
  </onecall:LocationDetails>
</onecall:OneCallReferral>
```
