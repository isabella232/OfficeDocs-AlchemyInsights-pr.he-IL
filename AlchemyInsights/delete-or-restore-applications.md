---
title: מחיקה או שחזור של יישומים
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102572"
---
# <a name="delete-or-restore-applications"></a>מחיקה או שחזור של יישומים

**כדי למחוק יישום מהדייר שלך ב- Azure AD**:

1. בפורטל **Azure AD**, בחר יישומים **ארגוניים**. לאחר מכן חפש ובחר את היישום שברצונך למחוק.
2. במקטע **ניהול** בחלונית הימנית, בחר **מאפיינים.**
3. בחר **מחק** ולאחר מכן בחר **כן כדי** לאשר שברצונך למחוק את היישום מהדייר שלך ב- Azure AD.

לקבלת מידע נוסף אודות אופן מחיקת יישום, ראה התחלה מהירה: מחיקת יישום מדייר [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

ב- PowerShell, [cmdlet Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) מסיר תצורות Proxy של יישום מיישום ספציפי ב- Azure Active Directory, והוא יכול למחוק את היישום לחלוטין אם צוין.

באפשרותך לשחזר **יישום שנמחק באמצעות** PowerShell. לאחר זיהוי היישום שברצונך לשחזר, באפשרותך לשחזר אותו באמצעות [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
