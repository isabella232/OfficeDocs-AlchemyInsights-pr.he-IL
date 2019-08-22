---
title: הפדרציה ADFS תפוגת התוקף של האישור
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
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499892"
---
# <a name="adfs-federation-certificate-expiring"></a>הפדרציה ADFS תפוגת התוקף של האישור

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את Microsoft תכלת הרקיע Active Directory מודול עבור Windows PowerShell במחשב (אם המודול אינו מותקן כבר). כדי לעשות זאת, עבור אל [ניהול AD תכלת הרקיע באמצעות Windows PowerShell](https://aka.ms/aadposh).

2. בצע את השלבים ב "תרחיש 1: פג תוקפו של האישור חתימת אסימון AD FS" מקטע של [השגיאה "אירעה בעיה בגישה אל האתר" מתוך AD FS כאשר משתמש מאוחד יוסיף ב- Office 365, תכלת הרקיע, או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. בצע את השלבים [בכיצד לעדכן או לתקן את ההגדרות של תחום מאוחד ב- Office 365, תכלת הרקיע, או Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    כדי ללמוד עוד אודות חידוש אישורים הפדרציה, ראה [חידוש אישורים הפדרציה עבור Office 365 ותכלת הרקיע Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
