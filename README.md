# Description
The DocsSpring connector allows Mendix users to complete activities in DocSpring without having to log into DocSpring. Features include:

* Create folders in your DocSpring account to organize PDF templates
* Create form templates by uploading a PDF
 * Templates will have entry fields automatically defined with a name, attribute type (Boolean, string, etc.) along with other important properties  
 * All attributes will have a defined field within which data will be positioned 
* Track document version history
* Generate test PDF documents with a watermark
* Submit completed documents to other systems of record
* Share completed documents with other systems (for example, eSignature platforms)

Link to DocSpring: https://docspring.com/

**Note:** You will be charged DocSpring rates per API call, as they have a pay-as-you-go model.

# Typical usage scenario

The DocSpring connector benefits anyone developing a case management system or document-related, in-app workflow.

At Entidad, we leverage the DocSpring connector to capture and submit PDF documents to United States Citizenship and Immigration Services (USCIS). Updated documents are submitted to the appropriate government agency, stored within a secure document vault, or sent to HelloSign to collect signatures.

# Features and limitations

* Create folders in your DocSpring account to organize PDF templates
* Create form templates by uploading a PDF
 * Templates will have entry fields automatically defined with a name, attribute type (Boolean, string, etc.) along with other important properties 
 * All attributes will have a defined field within which data will be positioned 
* Track document version history
* Generate test PDF documents with a watermark
* Submit completed documents to other systems of record
* Share completed documents with other systems (for example, eSignature platforms)

# Dependencies

* Mendix modeler version 9.12.5 or higher
* Must have an active DocSpring account
* Must have the Mendix Community Commons and Encryption modules

# Installation

* From within Mendix Studio Pro, navigate to the Mendix Marketplace (shopping cart icon)
* Download the Connector_DocSpring module from the Mendix Marketplace into your application
* Map the application’s roles to the module’s roles
* Explore the demo implementations by navigating to the DocSpring Connector’s Main Menu as an Administrator
* You’ll first need to set the API key in the Credentials configuration page

# Configuration

* Provide an active DocSpring API key and secret token

# Known bugs

N/A

# Frequently Asked Questions [optional]

**Q:** How do I create a new DocSpring template?

**A:** Create a DocSpring template either by uploading an existing PDF form using this DocSpring Connector or by manually creating one directly in DocSpring to your own specifications

**Q:** How do I populate data on a DocSpring template using my Mendix application?

**A:** Create a nonpersistent entity (NPE) with attribute names and types that match the DocSpring template’s attribute names and types. Populate the NPE attributes with your captured data, and then call the DocSpring Connector’s provided microflows to carry out your template actions, including API_TemplateUpdate and API_TemplateSubmit
