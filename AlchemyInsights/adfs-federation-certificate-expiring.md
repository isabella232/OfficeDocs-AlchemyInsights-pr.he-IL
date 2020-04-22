---
title: פג תוקפם של אישור הפדרציה של ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710408"
---
# <a name="adfs-federation-certificate-expiring"></a>פג תוקפם של אישור הפדרציה של ADFS

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את מודול מדריך ההפעלה התכלת של Microsoft עבור Windows PowerShell במחשב (אם המודול אינו מותקן כבר). כדי לעשות זאת, ללכת [לנהל לספירה תכלת באמצעות Windows PowerShell](https://aka.ms/aadposh).

2. בצע את השלבים בסעיף "תרחיש 1: תוקף האישור של חתימת האסימון של AD FS" של ["אירעה בעיה בגישה לאתר" מתוך AD fs כאשר משתמש מאוחד מתחבר ל-Microsoft 365, תכלת או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. בצע את השלבים ב [-Update או תקן את ההגדרות של תחום מאוחד ב-Microsoft, בתכלת או בIntune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    כדי ללמוד עוד אודות חידוש אישורי הפדרציה, ראה [חידוש אישורי הפדרציה עבור Microsoft 365 ו-"מדריך](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)כחול-פעיל".
