---
title: אישור האיחוד של ADFS עומד לפוג
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686715"
---
# <a name="adfs-federation-certificate-expiring"></a>אישור האיחוד של ADFS עומד לפוג

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את מודול Microsoft של Active Directory עבור Windows PowerShell במחשב (אם המודול אינו מותקן עדיין). לשם כך, עבור אל [ניהול AD תכולים באמצעות Windows PowerShell](https://aka.ms/aadposh).

2. בצע את השלבים המפורטים בסעיף "תרחיש 1: תוקף אישור האסימון לחתימה של AD FS" של ["אירעה בעיה בגישה לאתר" מתוך AD FS כאשר משתמש מאוחד נכנס ל-Microsoft 365, לתכלת או למנגינה](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. בצע את השלבים המפורטים [בעדכון או תיקון ההגדרות של תחום מאוחד ב-Microsoft, בתכלת או במנגינה](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    לקבלת מידע נוסף על חידוש אישורי איחוד, ראה [חידוש אישורי איחוד עבור Microsoft 365 ו-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
