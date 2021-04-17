---
title: תוקפו של אישור איחוד ADFS פג
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821952"
---
# <a name="adfs-federation-certificate-expiring"></a>תוקפו של אישור איחוד ADFS פג

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את מודול Microsoft Azure Active Directory עבור Windows PowerShell במחשב (אם המודול עדיין לא מותקן). לשם כך, עבור אל ניהול [Azure AD באמצעות Windows PowerShell](https://aka.ms/aadposh).

2. בצע את השלבים בסעיף "תרחיש 1: פג תוקפו של אישור חתימת אסימון של AD FS" של שגיאת "אירעה בעיה בגישה לאתר" מ- AD FS כאשר משתמש מאוחד נכנס ל- [Microsoft 365 , Azure או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. בצע את השלבים המפורטים בעדכון או תיקון ההגדרות של תחום מאוחד [ב- Microsoft , Azure או Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    לקבלת מידע נוסף על חידוש אישורי איחוד, ראה [חידוש אישורי איחוד עבור Microsoft 365 ו- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
