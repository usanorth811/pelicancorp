---
layout: default
title: Webhook
parent: Ticket Delivery Options
nav_order: 3
---

## Webhook
The full Webhook Utility Member Guides for both California and Nevada can be found using the links below.

<a href="https://usanorth811.org/images/USNCA-ONE-ANA-USA-North-811-Northern-California-TT55923-OneCallAccess-Webhook-Member-Guide.pdf" class="btn mr-4">California</a> <a href="https://usanorth811.org/images/USNNV-ONE-ANA-USA-North-811-Nevada-TT55923-OneCallAccess-Webhook-Member-Guide.pdf" class="btn mr-4">Nevada</a>

## Overview
The result of a request being created in OneCallAccess is a number of Notifications being created and sent to members of the service. A Member can choose to receive their Notifications via Web Hooks.

## Specifications
To use the Web Hook option, you need to provide a HTTPs endpoint to which OneCallAccess will send a JSON structure containing the relevant files that make up a Notification (XML, GML and GIF documents).
Members using this feature will need to provide the following values:

### URL
This is the URL which OneCallAccess will call for each Notification. The URL must accept a POST request. The URL must support HTTPS and must be reachable from the OneCallAccess environments.

### Secret Key
A secret string that allows the receiver to verify that the request was sent from OneCallAccess and that the body of the message has been unchanged.

### Custom HTTP headers (optional)
Some firewalls may require the inclusion of custom HTTP headers in requests to allow them to be proxied through the firewall.
OneCallAccess allows the inclusion of any number of custom HTTP headers in each Notification request (key/value).

##Payload
The payload is comprised of the message transmitted by OneCallAccess to the members of the external system. The following items are part of the payload:

### Header
- X-OneCall-Webhook-Signature (required) : sha256=<hashvalue>
- Content-Type (required) : application/json

### Request Body

```json
{
    "timestamp": "2921-09-14T07:44:10z,
    "webhookNotificationId": 1,
    "messageVersion": "1.0.0"
    "message": {
        "utilityId": 1,
        "utilityName": "Michigan State Authority",
        "stationCode": "MSA",
        "ticketNumber": "2021091401234-001"
        "sequenceNumber": 12,
        "requestDate": "2021-09-14T07:44:102"
        "XMLBase64" : "xxxxxxxxxxxxxxxxxxxxx",
        "GMLBase64" : "xxxxxxxxxxxxxxxxxxxxx",
        "GIFBase64" : "xxxxxxxxxxxxxxxxxxxxx"
     }
}
```

