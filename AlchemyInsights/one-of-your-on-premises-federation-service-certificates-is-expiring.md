---
title: אחד מאישורי שירות האיחוד המקומי עומד לפוג
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673498"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>אחד מאישורי שירות האיחוד המקומי עומד לפוג

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
- התקן את מודול Microsoft של Active Directory עבור Windows PowerShell במחשב (אם המודול אינו מותקן עדיין). לשם כך, עבור אל [תכלת Active Directory PowerShell עבור גרף ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- בצע את השלבים המפורטים בסעיף "תרחיש 1: תוקף אישור האסימון לחתימה של AD FS" של ["אירעה בעיה בגישה לאתר" מתוך AD FS כאשר משתמש מאוחד נכנס ל-Microsoft 365, לתכלת או למנגינה](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- בצע את השלבים המפורטים בנוגע [לעדכון או תיקון ההגדרות של תחום מאוחד ב-Microsoft 365, בתכלת או במנגינה](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
לקבלת מידע נוסף אודות חידוש אישורי איחוד, ראה [חידוש אישורים עבור O365 ו-תכלת לספירה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

