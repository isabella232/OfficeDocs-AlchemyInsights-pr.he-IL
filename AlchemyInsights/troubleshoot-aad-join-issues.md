---
title: פתרון בעיות הצטרפות ל- Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405126"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>פתרון בעיות הצטרפות ל- Azure AD

1. אם אתה מגדיר רישומי מכשירים בפעם הראשונה, ודא שסתכלת על מבוא לניהול מכשירים ב- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) שינחה אותך כיצד להשיג מכשירים תחת השליטה ב- Azure AD. 
1. אם אתה רושם מכשירים ל- Azure AD ישירות ורושם אותם ל- Intune, יהיה עליך לוודא שתצורת [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) נקבעה [והרשיון](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) יהיה במקום הראשון.
1. ודא שאתה מורשה לבצע פעולות ב- Azure AD. רק מנהל מערכת כללי ב- Azure AD יכול לנהל הגדרות עבור רישומי מכשירים.
1. כדי לעשות את יישום ההצטרפות של Azure AD, ראה [תכנון Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

לקבלת פרטים נוספים על פתרון בעיות נפוצות בצירוף Azure AD, ראה שאלות נפוצות בנושא [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) ובמכשיר Windows 10 pro, ראה אין אפשרות להצטרף למכשיר Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) ל- Azure AD - צורך לשדרג ל- Microsoft Community
