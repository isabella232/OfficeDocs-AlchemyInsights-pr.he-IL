---
title: הגדרת Outlook ברירת המחדל לא הוחלה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454754"
---
# <a name="default-outlook-label-setting-not-applied"></a>הגדרת Outlook ברירת המחדל לא הוחלה

אם הגדרות Outlook המוגדרות כברירת מחדל לא חלות כראוי, ולא מוחלת תווית אחרת או לא הוחלה תווית, ייתכן שאתה נתקל בבעיה ידועה (MC277818) ועליך לעשות אחת מ- 2 האפשרויות הבאות כדי לפתור את הבעיה:

**אפשרות 1:**

1. עבור אל Microsoft 365 תאימות מרכז > **פתרונות**  >  **הגנה על מידע**.
1. בחר **מדיניות תוויות** ובחר את מדיניות התוויות שתצטרך לערוך (**הגדרת OutlookDefaultlabel** אינה מוגדרת כראוי במדיניות התוויות הנוהרת. הפעל **את Get-labelpolicy** כדי להציג הגדרה זו) ולאחר מכן בחר **ערוך מדיניות**.
1. בחר **הבא** עד להגדרה החל תווית ברירת מחדל זו על הודעות דואר **אלקטרוני**, הזמינה אם תבחר דרוש מהמשתמשים להחיל תווית על הודעות דואר אלקטרוני ומסמכים **יורשים** בתיבת הדו-שיח **הגדרות** מדיניות.
1. בתיבת **הדו-שיח החלת תווית ברירת** מחדל על מסמכים, **בחר ללא** מהרשימה הנפתחת.
1. בחר **הבא** ושלח **כדי** לשמור את הגדרות התוויות.

**אפשרות 2:**

ב- [Powershell של מרכז האבטחה והתאימות,](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)השתמש בפקודה Set-LabelPolicy כדי לשנות את **OutlookDefaultlabel** **ללא ב-** {OutlookDefaultLabel="None"}.

הפעל: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

לקבלת מידע נוסף אודות תוויות ברירת מחדל עבור Outlook, ראה [הגדרת תווית ברירת מחדל אחרת עבור Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)