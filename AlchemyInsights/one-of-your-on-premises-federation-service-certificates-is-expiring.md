---
title: תוקפו של אחד מאישורי שירות האיחוד המקומיים שלך פג
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810053"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>תוקפו של אחד מאישורי שירות האיחוד המקומיים שלך פג

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
- התקן את מודול Microsoft Azure Active Directory עבור Windows PowerShell במחשב (אם המודול עדיין לא מותקן). לשם כך, עבור אל [Azure Active Directory PowerShell עבור Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- בצע את השלבים בסעיף "תרחיש 1: פג תוקפו של אישור חתימת אסימון של AD FS" של שגיאת "אירעה בעיה בגישה לאתר" מ- AD FS כאשר משתמש מאוחד נכנס ל- [Microsoft 365 , Azure או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- בצע את השלבים המפורטים כיצד לעדכן או לתקן את ההגדרות של תחום מאוחד [ב- Microsoft 365 , Azure או Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
לקבלת מידע נוסף אודות חידוש אישורי איחוד, ראה חידוש [אישורים עבור O365 ו- Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

