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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952970"
---
# <a name="adfs-federation-certificate-expiring"></a>תוקפו של אישור איחוד ADFS פג

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את Microsoft Azure Active Directory המודול Windows PowerShell במחשב (אם המודול עדיין לא מותקן). לשם כך, עבור אל ניהול [Azure AD באמצעות Windows PowerShell](https://aka.ms/aadposh).

2. בצע את השלבים המפורטים בסעיף "תרחיש 1: פג תוקפו של אישור חתימת אסימון של AD FS" של שגיאת "אירעה בעיה בגישה לאתר" מ- AD FS כאשר משתמש מאוחד נכנס ל- [Microsoft 365, Azure או Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. בצע את השלבים המפורטים בעדכון או תיקון ההגדרות של תחום מאוחד [ב- Microsoft , Azure או Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    לקבלת מידע נוסף על חידוש אישורי איחוד, ראה [חידוש אישורי איחוד עבור Microsoft 365 ו- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
