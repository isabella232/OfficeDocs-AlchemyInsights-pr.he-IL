---
title: Troubleshoot Hybrid Azure AD join
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401908"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Troubleshoot Hybrid Azure AD join

מומלץ מאוד לוודא שמכשיר יכול לגשת לנקודות קצה לרישום מכשיר תחת חשבון המערכת באמצעות [קובץ ה- Script של בדיקת קישוריות רישום מכשיר](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. אם אתה מגדיר רישומי מכשירים בפעם הראשונה, הקפד לעיין ב[מבוא לניהול מכשירים ב- Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) כדי ללמוד כיצד לקבל מכשירים בשליטת Azure AD.
1. אם אתה רושם מכשירים ל- Azure AD ישירות ורושם אותם ל- Intune, ודא תחילה ש[קבעת את התצורה של Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ושיש לך [רשיון](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. ודא שאתה מורשה לבצע פעולות ב- Azure AD וב- AD מקומי. רק מנהל מערכת כללי ב- Azure AD יכול לנהל הגדרות עבור רישומי מכשירים. בנוסף, אם אתה מגדיר רישומים אוטומטיים ב- Active Directory המקומי שלך, יהיה עליך להיות מנהל מערכת של Active Directory ו- AD FS (אם רלוונטי).

לקבלת פרטים נוספים על פתרון בעיות פוטנציאליות ב- Hybrid join, ראה [פתרון בעיות ב- Hybrid join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) עבור הגדרת משתמש ב- hybrid Azure AD join וניהול מכשירים באמצעות פורטל Azure Ad, ראה [הגדרת מכשירי משתמש ב- hybrid Azure AD join (מכשירי join של תחום מקומי)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ו[ניהול מכשירים באמצעות פורטל Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

כדי לפתור בעיות נפוצות ב- Hybrid Azure Active Directory (AD) join, ראה שאלות נפוצות על [שאלות נפוצות בנושאHybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
