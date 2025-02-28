---
title: "Alternative Ways to Get a Data Connection (Report Builder) | Microsoft Docs"
description: Learn details about alternative ways to connect to an external data source, such as a SQL Server database.
ms.date: 06/15/2016
ms.service: reporting-services
ms.subservice: reporting-services

ms.topic: conceptual
ms.assetid: aebc5f3d-97d5-4d54-b525-753fed073a9a
author: maggiesMSFT
ms.author: maggies
---
# Alternative Ways to Get a Data Connection (Report Builder)
A data connection contains the information to connect to an external data source such as a [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] database. Usually, you get the connection information and the type of credentials to use from the data source owner.  
  
To specify a data connection, you can use a shared data source from the report server or create an embedded data source that is used only in a specific report.  
  
In most tutorials you use embedded data sources, but if you have access to shared data sources, then you can use them instead.  
  
## Getting a Data Connection From a Shared Data Source  
If the report server has available shared data sources that you have permission to use, you can use them instead of an embedded data source. The following procedures tell how to locate the shared data sources and provide any credentials needed to use them.  
  
To use a shared data source, you browse to a report server and select one. Usually, you get the report server URL from the report server administrator.  
  
### To specify a data connection from a list of shared data sources  
  
1.  In the New Table or Matrix or the New Chart Wizard, on the **Choose a dataset** page, select **Create a dataset**, and then click **Next**. The **Choose a connection to a data source** page opens.  
  
2.  From the list of data sources, select a data source that you have permission to access.  
  
3.  To verify that you can connect to the data source, click **Test Connection**. The message "Connection created successfully" appears. Select **OK**.
  
4.  Click **Next**.  
  
    If necessary, enter your credentials. To save the credentials locally, select **Save password with connection**. If you don't select this option, you will be prompted for credentials every time that you run the report  
  
5.  Select **OK**.
  
### To specify a data connection by browsing to a shared data source on a report server  
  
1.  In the New Table or Matrix or the New Chart Wizard, on the **Choose a dataset** page, select **Create a dataset**, and then click **Next**. The **Choose a connection to a data source** page opens.  
  
2.  Click **Browse**. The **Select Data Source** dialog box opens.  
  
3.  From the **Look in** drop-down list, select **Recent Sites and Servers**. In the data source pane, click the URL for your server, and then click **Open**.  
  
    The list of data sources or models appears.  
  
4.  Alternatively, in **Name**, type the URL to the report server. Click **Open**.  
  
    Report Builder connects to the report server and loads the data sources that are available at the root folder.  
  
5.  Navigate to a folder that contains a data source that you have sufficient permissions to connect to, select the data source, and then click **Open**.  
  
    You are back on the **Choose a connection to a data source** page.  
  
6.  To verify that you can connect to the data source, click **Test Connection**.  
  
    The message "Connection created successfully" appears. Select **OK**.
  
7.  Click **Next**.  
  
8.  If you are prompted for a user name and password, enter your credentials. To save the credentials locally, select **Save password with connection**.  
  
9. Select **OK**.
  
## See Also  
[Report Datasets &#40;SSRS&#41;](../reporting-services/report-data/report-datasets-ssrs.md)  
[Report Builder Tutorials](../reporting-services/report-builder-tutorials.md) 
  

