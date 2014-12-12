# SAP (JCO) Knowledge Sensor Pack

## Overview

This Knowledge Sensor Pack can be used to help quantify and diagnose performance issues related to usage of a JCO/ABAP calls from within SAP.

## Plugin Details

| Name | SAP (JCO) Knowledge Sensor Pack
| :--- | :---
| Author | dynaTrace software
| Supported dynaTrace Versions | >= 5.5
| Supported JCO Versions | SAP JCO v2.1.7
| License | [dynaTrace BSD](dynaTraceBSD.txt)
| Support | [Community](https://community.compuwareapm.com/community/display/DL/Support+Levels#SupportLevels-Community)
| Release history | Version 1.1
| Download | [com.sap.mpw.jco.Remoting.SAP_Java_Connector.dtcs](com.sap.mpw.jco.Remoting.SAP_Java_Connector.dtcs)


## Installation

  1. Save the attached file locally to the computer where the dynaTrace Diagnostics Client is installed. 

  2. In the dynaTrace Client, choose _Setting ⇒ dynaTrace Server Settings_

  3. Click on "Sensor Packs". 

  4. Click on the "Import..." button. 

  5. Select "Custom Sensor Type (*.dtcs)" in the "Files of type" dropdown. 

  6. Navigate to the directory where you extracted the .dtcs file and click "Open". 

You can confirm successful import by observing the "Spring Sensor" Sensor Pack in the Sensor Packs Panel. This Knowlege Sensor Pack is now _Placed_ and _Active_ within all System Profiles on this
dynaTrace Server.

Note:

There is no visibility into the internals of ABAP calls, however by monitoring the JCO calls, the cost of calls from Java into ABAP can be measured and provide visibility into which ABAP calls are
potentially causing problems.

Note: This Knowledge Sensor Pack has been updated to handle SAP JCO v2.1.7. This involved adding support for the class com.sap.mw.jco.JCO$Client. Prior, the only class which was covered was
com.sap.mw.jco.Client. Same methods are used on both classes.

