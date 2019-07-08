---
layout: default
title: Overview
nav_order: 1  
---
###### [\| Download PDF \|](docs\assets\DigitalPersona Access Management API.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[\| View Repo \|](https://github.com/LenHodgeman/digitalpersona-access-management-api/)&nbsp;&nbsp;&nbsp;&nbsp;| REVIEW DRAFT  |  
[//]: #(<--\| DRAFT A154 \|  -->)  

![](docs/assets/HID-logo.png)  

## Overview  

The DigitalPersona Access Management API provides a comprehensive set of components and libraries exposing various functions and methods for using the power of the DigitalPersona platform in your own custom-built web-based and native Windows applications.  

Sample programs are also provided, which illustrate the features available through the included APIs.  

This documentation is divided into several sections that align with the specific uses of the various components, APIs and wrappers available.

To read an overview of each section, on desktop browsers, use the links on the left. For mobile browsers, use the Menu button at the top of the screen.

To go directly to detailed documentation on an item, use the links below to view the GitHub Pages documentation provided with the item's repository. Links to each repository are provided on the first page of its documentation.

<table style="width:95%;margin-left:auto;margin-right:auto;">
  <tr>
    <th style="width:20%" ALIGN="left">Section</th>
    <th style="width:35%" ALIGN="left">Repository & documentation</th>
    <th style="width:45%" ALIGN="left">Purpose</th>
  </tr>
  <tr>
  <td valign="top" >Components</td>
  <td valign="top" ><A HREF="https://lenhodgeman.github.io/digitalpersona-core/index.html">digitalpersona-core</A></td>
    <td>Contains the core classes and functions shared by the Access Management APIs.</td>
  </tr>
  <tr>
    <td>&nbsp;</td>
    <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-services/index.html">digitalpersona-services</A></td>
    <td>JS wrappers for the Web Access Services shared by the authentication and enrollment APIs</td>
  </tr>
  <tr>
    <td>&nbsp;</td>
    <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-access-management-services/index.html">digitalpersona-access-management-services</A></td>
    <td>[TBD]</td>
  </tr>  
  <tr>
  <td>&nbsp;</td>
  <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-authentication/index.html">digitalpersona-authentication</A></td>
    <td>API enabling credential authentication</td>
  </tr>
  <tr>
      <td>&nbsp;</td>
      <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-enrollment/index.html">digitalpersona-enrollment</A></td>
    <td>API enabling credential enrollment</td>
  </tr>
  <tr>
      <td>&nbsp;</td>
    <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-devices/index.html">digitalpersona-devices</A></td>
    <td>API providing access to devices supported by the DigitalPersona Access Mangement API.</td>
  </tr>
  <tr>
      <td>&nbsp;</td>
    <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-native-api/index.html">digitalpersona-native-api</A></td>
    <td>API providing native Windows implementation of enrollment, authentication and device access.</td>
  </tr>
  <tr>
    <td  valign="top">Sample Applications</td>
    <td  valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-web-sample/index.html">digitalpersona-javascript-sample-application</A></td>
    <td>Sample web application illustrating web authentication, enrollment and device access.</td>
  </tr>
  <tr>
    <td  valign="top">&nbsp;</td>
    <td  valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-web-sample/index.html">digitalpersona-web-sample</A></td>
    <td>Sample application illustrating web authentication, enrollment and device access.</td>
  </tr>
  <tr>
    <td  valign="top">&nbsp;</td>
    <td  valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-web-sample/index.html">digitalpersona-oidc-sample</A></td>
    <td>Sample application using OpenID Connect that illustrates web authentication, enrollment and device access.</td>
  </tr>
  <tr>
    <td valign="top">&nbsp;</td>
    <td valign="top"><A HREF="https://lenhodgeman.github.io/digitalpersona-native-samples/index.html">digitalpersona-native-samples</A></td>
    <td valign="top">Sample native Windows applications in C++ and .NET, illustrating Windows enrollment, authentication and device access.</td>
  </tr>
</table>

For web-based applications, you can use the Authentication or Enrollment APIs directly, or through the relevant JavaScript wrappers to enroll and authenticate DigitalPersona users quickly and easily against authentication policies as defined by the DigitalPersona administrator or through custom policies defined by your application, and subsequently release their users’ protected data (secrets).

For Windows native applications, the Native API provides an API which can accessed through either C++ or .NET applications.

All of the authentication credentials provided in the DigitalPersona solution are supported through the corresponding APIs except for the Face credential (for web APIs) and the Bluetooth credential (web and Windows APIs).

## Working environment
Use of the included APIs assumes that an appropriate DigitalPersona solution has been installed, configured and verified. Features exposed through the Native APIs can be used in a minimal DigitalPersona environment consisting of the DigitalPersona Workstation or DigitalPersona Kiosk and a single DigitalPersona AD or LDS Server. Use of the REST APIs requires the additional installation of the DigitalPersona Web Components package.

## Target Audience
Developers should have an understanding of the core components of the DigitalPersona solution and its terminology and concepts. They should also be knowledgeable in the specific target platform and the relevant development language.

## Additional Resources
You can refer to the additional resources described in this section to assist you in using the API.  

<table style="width:100%;margin-left:auto;margin-right:auto;">
  <tr>
    <th style="width:50%" ALIGN="left">Subject</th>
    <th style="width:50%" ALIGN="left">Resource</th>
  </tr>
  <tr>
    <td valign="top" >Concepts, features, processes and terminology used in DigitalPersona solutions</td>
    <td valign="top">DigitalPersona AD and LDS Administrator Guides, Client Guide and supporting documentation is available at: <A HREF="https://www.crossmatch.com/company/support/documentation">https://www.crossmatch.com/company/support/documentation </A></td>
  </tr>
</table>

## System Requirements
### Development system
#### REST APIs
In addition to the requirements listed above, the following are required for use of the Web AUTH and Web Enrollment APIs.

* Windows Web Server (IIS)

* DigitalPersona Web Management Components

* An SSL certificate

See the DigitalPersona Administrator and Client Guides for instructions on installing and configuring the above components.  

#### Native API
The recommended minimum software requirements needed to develop applications with the DigitalPersona Native API are:
* Development workstation running Windows 7 or later and DigitalPersona Workstation or Kiosk.

* To compile the sample code: Visual Studio 2008 or later.
DigitalPersona Server running Windows Server 2012 and DigitalPersona AD or LDS Server.

* DigitalPersona Server running Windows Server 2012 and DigitalPersona AD or LDS Server.

See the topic *Supported DigitalPersona Products* below for a complete list of compatible DigitalPersona clients and servers.

### Target system

Recommended minimum software requirements are the same as for the development system with the following exceptions:

* Visual Studio is not required.

* DigitalPersona Server running Windows Server 2012 and DigitalPersona AD or LDS Server.

* If the logon and Password Manager features are not needed, the DigitalPersona client can be installed without these applications. This installs the DigitalPersona Access Management API runtime only.

## Supported DigitalPersona Products

The DigitalPersona Access Management API is compatible with the following DigitalPersona products:

* DigitalPersona AD or LDS Workstation 2.1 or later.

* DigitalPersona AD or LDS Kiosk 2.1 or later.

* DigitalPersona AD or LDS AD Server, version 2.1 or later.
