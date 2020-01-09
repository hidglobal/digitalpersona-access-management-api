---
layout: default
title: Overview
nav_order: 1  
---

{% include header.html %}
<BR>

# Overview

The DigitalPersona Access Management API provides a comprehensive set of components and libraries exposing various functions and methods for using the power of the DigitalPersona platform in your own custom-built web-based and native Windows applications.  

Sample programs, listed in the table below, are also provided, which illustrate the features available through the included APIs.  

This documentation is divided into several sections that align with the specific uses of the various components, APIs and wrappers available.

* To read a brief overview of each section, on desktop browsers, use the links on the left. For mobile browsers, use the Menu button at the top of the screen.

* To read the provided documentation for an item, use the links below.
* To go to the actual repository, click the [View Repo] link in the upper-right corner of any page within the section's documentation.

<table style="width:95%;margin-left:auto;margin-right:auto;">
  <tr>
    <th style="width:20%" ALIGN="left">Category</th>
    <th style="width:35%" ALIGN="left">Component&nbsp;or&nbsp;Sample</th>
    <th style="width:45%" ALIGN="left">Purpose</th>
  </tr>
  <tr>
  <td valign="top" >Components</td>
  <td valign="top" ><A HREF="https://hidglobal.github.io/digitalpersona-core/index.html">DigitalPersona API Core</A></td>
    <td>Contains the core classes and functions shared by the Access Management APIs.</td>
  </tr>
  <tr>
    <td>&nbsp;</td>
    <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-services/index.html">Web Access Services API</A></td>
    <td>JS wrappers for the Web Access Services shared by the authentication and enrollment APIs</td>
  </tr>
  <tr>
    <td>&nbsp;</td>
    <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-access-management-services/index.html">Access Management Services API</A></td>
    <td>A collection of RESTful services used to implement various features of the DigitalPersona solution in web applications.</td>
  </tr>  
  <tr>
  <td>&nbsp;</td>
  <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-authentication/index.html">Credential Authentication API</A></td>
    <td>API enabling credential authentication</td>
  </tr>
  <tr>
      <td>&nbsp;</td>
      <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-enrollment/index.html">Web credential enrolllment API</A></td>
    <td>API enabling web-based credential enrollment</td>
  </tr>
  <tr>
      <td>&nbsp;</td>
    <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-devices/index.html">Device Access API</A></td>
    <td>API providing access to devices supported by the DigitalPersona Access Mangement API.</td>
  </tr>
  <tr>
      <td>&nbsp;</td>
    <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-native-api/index.html">Windows native API</A></td>
    <td>API providing native Windows implementation of enrollment, authentication and device access.</td>
  </tr>
  <tr>
    <td  valign="top">Sample Applications</td>
    <td  valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-sample-web/">DigitalPersona Web demo</A></td>
    <td>Sample program (DPWebDemo.exe) that creates a GUI displaying fields and buttons that showcase the primary features of the DigitalPersona Web Enrollment Services API.</td>
  </tr>
  <tr>
    <td  valign="top">&nbsp;</td>
    <td  valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-sample-angularjs/">Bank of DigitalPersona sample</A></td>
    <td>Sample website demonstrating typical DigitalPersona Web Access Management API use cases through a fictional Bank of Digitalpersona.</td>
  </tr>
  <tr>
    <td  valign="top">&nbsp;</td>
    <td  valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-sample-js-oidc/">OpenID Connect sample</A></td>
    <td>Sample JavaScript application using OpenID Connect and illustrating web authentication, enrollment and device access.</td>
  </tr>
  <tr>
    <td valign="top">&nbsp;</td>
    <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-sample-dotnet/">Native Windows .NET sample</A></td>
    <td valign="top">.NET sample code for the DigitalPersona Access Management API (Native API)</td>
  </tr>
  <tr>
    <td valign="top">&nbsp;</td>
    <td valign="top"><A HREF="https://hidglobal.github.io/digitalpersona-sample-cpp/">Native Windows C++ sample</A></td>
    <td valign="top">C++ sample code for the DigitalPersona Access Management API (Native API)</td>
  </tr>
</table>

For web-based applications, you can use the higher-level Authentication and  Enrollment APIs, or more directly through the RESTful services themselves, to enroll and authenticate DigitalPersona users quickly and easily against authentication policies as defined by the DigitalPersona administrator or through custom policies defined by your application, and subsequently release their users’ protected data (secrets).

For Windows native applications, the Native API provides an API which can accessed through either [C++](https://hidglobal.github.io/digitalpersona-sample-cpp/index.html) or [.NET](https://hidglobal.github.io/digitalpersona-sample-dotnet/index.html) applications.

All of the authentication credentials provided in the HID DigitalPersona solution are supported through the corresponding APIs except for the Face credential (for web APIs) and the Bluetooth credential (web and Windows APIs).

# Working environment
Use of the included APIs assumes that an appropriate HID DigitalPersona solution has been installed, configured and verified. Features exposed through the Native APIs can be used in a minimal HID DigitalPersona environment consisting of the HID DigitalPersona Workstation or HID DigitalPersona Kiosk and a single HID DigitalPersona AD or LDS Server. Use of the REST APIs requires the additional installation of the HID DigitalPersona Web Components package.

# Target Audience
Developers should have an understanding of the core components of the HID DigitalPersona solution and its terminology and concepts. They should also be knowledgeable in the specific target platform and the relevant development language.

# Additional Resources
You can refer to the additional resources described in this section to assist you in using the API.  

<table style="width:100%;margin-left:auto;margin-right:auto;">
  <tr>
    <th style="width:50%" ALIGN="left">Subject</th>
    <th style="width:50%" ALIGN="left">Resource</th>
  </tr>
  <tr>
    <td valign="top" >Concepts, features, processes and terminology used in HID DigitalPersona solutions</td>
    <td valign="top">HID DigitalPersona AD and LDS Administrator Guides, Client Guide and supporting documentation is available at: <A HREF="https://www.crossmatch.com/company/support/documentation">https://www.crossmatch.com/company/support/documentation </A></td>
  </tr>
</table>

# System Requirements
The following section describes the requirements for the Development System and the Target System.
## Development system
The following section describes the requirements for the Development System.
### REST APIs
In addition to the requirements listed above, the following are required for devlopment with the Web AUTH and Web Enrollment APIs.

* Windows Web Server (IIS)
* HID DigitalPersona Web Management Components
* An SSL certificate

See the HID DigitalPersona Administrator and Client Guides for instructions on installing and configuring the above components.  

### Native API
The recommended minimum software requirements needed to develop applications with the DigitalPersona Native API are:
* Development workstation running Windows 7 or later and HID DigitalPersona Workstation or Kiosk.
* To compile the sample code: Visual Studio 2012 or later.
HID DigitalPersona Server running Windows Server 2012 and HID DigitalPersona AD or LDS Server.
* HID DigitalPersona Server running Windows Server 2012 and HID DigitalPersona AD or LDS Server.

See the topic *Supported HID DigitalPersona Products* below for a complete list of compatible HID DigitalPersona clients and servers.

## Target system
The following section describes the requirements for the Target System. Recommended minimum software requirements are the same as for the development system with the following exceptions:

* Visual Studio is not required.
* HID DigitalPersona Server running Windows Server 2012 and HID DigitalPersona AD or LDS Server.
* If the logon and Password Manager features are not needed, the HID DigitalPersona client can be installed without these applications. This installs the DigitalPersona Access Management API runtime only.

# Supported HID DigitalPersona Products

The DigitalPersona Access Management API is compatible with the following HID DigitalPersona products:

* DigitalPersona AD or LDS Workstation 3.1 or later.
* DigitalPersona AD or LDS Kiosk 3.1 or later.
* DigitalPersona AD or LDS AD Server, version 3.1 or later.
