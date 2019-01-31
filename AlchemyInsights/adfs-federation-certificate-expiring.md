---
title: הפדרציה ADFS תפוגת התוקף של האישור
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 6170265dac1eebe8fa1acf766d2eb8d6b0a5908b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662364"
---
# <a name="adfs-federation-certificate-expiring"></a>הפדרציה ADFS תפוגת התוקף של האישור

כדי לפתור בעיה זו, בצע את הפעולות הבאות:
  
1. התקן את Microsoft תכלת הרקיע Active Directory מודול עבור Windows PowerShell במחשב (אם המודול אינו מותקן כבר). כדי לעשות זאת, עבור אל [ניהול AD תכלת הרקיע באמצעות Windows PowerShell](https://aka.ms/aadposh).
    
2. בצע את השלבים ב "תרחיש 1: פג תוקפו של האישור חתימת אסימון AD FS" מקטע של [השגיאה "אירעה בעיה בגישה אל האתר" מתוך AD FS כאשר משתמש מאוחד יוסיף ב- Office 365, תכלת הרקיע, או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. בצע את השלבים [בכיצד לעדכן או לתקן את ההגדרות של תחום מאוחד ב- Office 365, תכלת הרקיע, או Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    כדי ללמוד עוד אודות חידוש אישורים הפדרציה, ראה [חידוש אישורים הפדרציה עבור Office 365 ותכלת הרקיע Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

