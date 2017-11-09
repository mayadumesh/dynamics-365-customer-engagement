---
title: "Keep your data in Dynamics 365 for Sales, Business edition clean with duplicate detection | Microsoft Docs"
description: "Enable duplicate detection in Dynamics 365 for Sales, Business edition to keep your sales data clean."
keywords: "Duplicate; Enable; Disable"
author: shubhadaj
ms.author: shujoshi
manager: sakudes
applies_to: "Dynamics 365 (online)"
ms.date: 07/14/2017
ms.service: dynamics-365
ms.topic: article
ms.assetid: 83bdaae9-1f72-45d5-b4c2-bd0a070a9c05
ms.reviewer: 
---

# Keep your data clean with duplicate detection

[!INCLUDE[Pre-release disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

To maintain the integrity of your data, it’s a good idea to set up duplicate detection to detect duplicate records in the system. By default, duplicate detection is already enabled for [!INCLUDE[pn-ms-dyn-365-for-sales](../includes/pn-ms-dyn-365-for-sales.md)].

## Duplicate detection rules

[!INCLUDE[pn-ms-dyn-365-for-sales](../includes/pn-ms-dyn-365-for-sales.md)] includes duplicate detection rules for accounts and contacts. The rules are automatically published when duplicate detection is enabled.

-   Accounts with the same account name are found

-   Contacts with the same first name and last name are found

-   Contacts with the same email address are found

If any of these rules is deleted, duplicate detection won’t work as expected.

## Enable Duplicate Detection

If duplicate detection is disabled, duplicates won’t be detected.

To enable duplicate detection

1. Go to **Advanced** **Settings** &gt; **Duplicate** **Detection**.

2.  Click **Enable**.

## When does duplicate detection happen?

If duplicate detection is enabled, duplicates are detected when:

 - **A record is created or updated**

 The system checks for duplicates when a user enters or updates records.
  
 > [!Important]
 
 > Duplicates aren’t detected when a user merges two records, activates or deactivates a record, or saves a completed activity.
 
 - **During data import**
 
 When you use the Import Data wizard to bring in contacts or accounts the wizard detects any duplicate records.

## Disable duplicate detection

If your system contains a large number of records, checking for duplicates can impact performance. You may want to disable duplicate detection at such times.

1.  To disable duplicate detection, go to **Advanced Settings** &gt; **Duplicate Detection**.

2.  Click **Disable**.

All the duplicate detection rules will be unpublished in the backend.


### See Also
[Import data into [!INCLUDE[pn-ms-dyn-365-for-sales](../includes/pn-ms-dyn-365-for-sales.md)]](import-data.md)  
[Set up the Sales app for your team](set-up-sales-app-team.md)
