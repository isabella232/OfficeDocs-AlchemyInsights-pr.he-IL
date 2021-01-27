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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014900"
---
# <a name="delete-or-restore-applications"></a>מחיקה או שחזור של יישומים

**כדי למחוק יישום מהדיירים של תכלת לספירה**:

1. בפורטל **תכלת לספירה**, בחר **יישומים ארגוניים**. לאחר מכן, אתר את היישום שברצונך למחוק ובחר אותו.
2. במקטע **ניהול** בחלונית הימנית, בחר **מאפיינים**.
3. בחר באפשרות **מחק** ולאחר מכן בחר **כן** כדי לאשר שברצונך למחוק את היישום מדייר ה-תכלת לספירה.

לקבלת מידע נוסף אודות האופן שבו ניתן למחוק יישום, ראה [תחלה: מחיקת יישום מהדיירים של ' תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

ב-PowerShell, ה [-Cmdlet Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) מסיר תצורות Proxy של יישומים מיישום ספציפי ב-תכלת Active Directory, ויכול למחוק את היישום לגמרי אם צוין.

באפשרותך **לשחזר יישום שנמחק** באמצעות PowerShell. ברגע שהיישום שברצונך לשחזר זוהה, באפשרותך לשחזר אותו באמצעות [שחזור-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
