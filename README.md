[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/abap-alv-google-upload-sheet)](https://api.reuse.software/info/github.com/SAP-samples/abap-alv-google-upload-sheet)

# Integration of Google Sheets into ABAP List Viewer

## Important note before starting your project setup/configuration
We are happy to announce that Google Cloud and SAP have expanded their partnership to enable a native integration between Google Workspace and SAP S/4HANA. Our customers now have the possibility to export data from all important UI Tables to Google Sheets as well as a table import from Google Sheets to the Upload General Journal Entries application. This initial set of features is included in **SAP S/4HANA Cloud 2208 and S/4HANA 2022**, leveraging an SAP Business Technology Platform service (additional license required: SAP Document Management Service, integration option). 

Please feel free to check out our [public documentation and set-up guide](https://help.sap.com/docs/DOCUMENT_MANAGEMENT/f6e70dd4bffa4b65965b43feed4c9429/594bf95dbab64358aef97a73296b6054.html) as well as our
blog posts:
- [Seamless integration between SAP S/4HANA & Google Workspace](https://community.sap.com/t5/enterprise-resource-planning-blogs-by-sap/seamless-integration-between-sap-s-4hana-google-workspace/ba-p/13535025)
- [SAP’s UI Technologies enabling Google Workspace](https://community.sap.com/t5/technology-blogs-by-sap/sap-s-ui-technologies-enabling-google-workspace/ba-p/13540756)

## Project Description
This project comprises an archive containing sample source code for the integration of Google Sheets into the ABAP List Viewer (ALV) component. Thus, this sample code helps you to implement and configure the export of ALV grid data from SAP GUI directly to Google Drive and display exported data snapshots automatically in Google Sheets.

## Minimum Requirements

- This functionality is only available for certain SAP NetWeaver support packages, see [note 2592115](http://service.sap.com/sap/support/notes/2592115).
- After installation of the corresponding Support Package, it is **mandatory** to implement [note 2624404](http://service.sap.com/sap/support/notes/2624404) (ALV GUI: BAdi Export Integration Corrections).

## Download and Installation

### Proceed as follows to make best use of the sample code:

1. Clone the repository or use the [abapGit client](https://docs.abapgit.org/) to [import](https://docs.abapgit.org/guide-import-zip.html) the sources into your SAP system.
2. Setup the Google API Endpoint (see chapter 2.2 in [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html) )
3. Create a Service Provider Type for Google (see chapter 2.3.1 [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html))
4. Create an OAuth 2.0 Client Profile (see chapter 2.3.6 [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html))
5. Configure the Access to Google APIs (see chapter 2.4 [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html))
6. Check the Connection (see chapter 2.5. [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html))
7. ALV ABAP administration (see chapter 3.2 [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html))

## Configuration Guide

See the full documentation [Export of ALV Grid Data to Google Sheets](https://www.sap.com/documents/2018/07/56e0dd6d-0f7d-0010-87a3-c30de2ffd8ff.html) available in the SAP Community.

## Limitations

- The redirect URL called by Google requires a public top level domain server. 
- There is no way to use an Enterprise account or logon to Google Drive via SSO  – every end user needs a regular Google account.

## Known Issues

None.

## How to obtain support

**No SAP standard support** provided: Consult **SAP [note 2896606](http://service.sap.com/sap/support/notes/2896606) for details**.

You can ask your questions concerning this functionality in the [SAP Community](https://www.sap.com/community.html). Please, use _ABAP Development_ as primary tag and choose _alv_ as additional user tag.

You find an overview of all ALV questions under: [https://answers.sap.com/topics/alv.html](https://answers.sap.com/topics/alv.html).

## Contribution

An SAP Code Sample such as this is open software but is not quite a typical full-blown open source project. If you come across a problem, we’d encourage you to check the project’s [issue tracker](https://github.com/SAP-samples/abap-alv-google-upload-sheet/issues) and to [file a new issue](https://github.com/SAP-samples/abap-alv-google-upload-sheet/issues/new) if needed. If you are especially passionate about something you’d like to improve, you are welcome to fork the repository and submit improvements or changes as a pull request.

## License
Copyright (c) 2021 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.

Note that the sample code includes calls to the Google Drive APIs which calls are licensed under the Creative Commons Attribution 3.0 License _(_[_https://creativecommons.org/licenses/by/3.0/_](https://creativecommons.org/licenses/by/3.0/)_)_ in accordance with Google&#39;s Developer Site Policies _(_[_https://developers.google.com/terms/site-policies_](https://developers.google.com/terms/site-policies)_)._ Furthermore, the use of the Google Drive service is subject to applicable agreements with Google Inc.
