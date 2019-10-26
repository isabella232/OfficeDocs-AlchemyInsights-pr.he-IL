---
title: פג תוקפם של אישור הפדרציה של ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737190"
---
# <a name="adfs-federation-certificate-expiring"></a>פג תוקפם של אישור הפדרציה של ADFS

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את מודול מדריך ההפעלה התכלת של Microsoft עבור Windows PowerShell במחשב (אם המודול אינו מותקן כבר). כדי לעשות זאת, ללכת [לנהל לספירה תכלת באמצעות Windows PowerShell](https://aka.ms/aadposh).

2. בצע את השלבים בסעיף "תרחיש 1: תוקף האישור של חתימת האסימון של AD FS" של ["אירעה בעיה בגישה לאתר" מתוך AD fs כאשר משתמש מאוחד מתחבר ל-Office 365, תכלת או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. בצע את השלבים [בעדכון או תקן את ההגדרות של תחום מאוחד ב-Office 365, תכלת או Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    כדי ללמוד עוד אודות חידוש אישורי הפדרציה, ראה [חידוש אישורי הפדרציה עבור Office 365 ו-"כחול פעיל](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)".
