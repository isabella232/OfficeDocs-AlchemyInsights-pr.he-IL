---
title: פתרון בעיות במסירת דואר אלקטרוני לתיקיות ציבוריות התומכות בדואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068813"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>פתרון בעיות במסירת דואר אלקטרוני לתיקיות ציבוריות התומכות בדואר

אם שולחים חיצוניים לא יכולים לשלוח הודעות לתיקיות הציבוריות התומכות בדואר, והשולחים מקבלים את השגיאה: לא היתה אפשרות למצוא **(550 5.4.1)**, ודא שתחום הדואר האלקטרוני עבור התיקיה הציבורית מוגדר כתחום תחום ממסר פנימי במקום כתחום סמכותי:

1. פתח את [Exchange הניהול של מרכז הניהול (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. עבור אל **תחומים** \> **מקובלים של זרימת דואר**, בחר את התחום המקובל ולאחר מכן לחץ על **ערוך**.

3. בדף המאפיינים שנפתח, אם סוג התחום מוגדר ל'סמכותי', שנה את הערך לממסר **פנימי** ולאחר מכן לחץ על **שמור**.

אם שולחים חיצוניים מקבלים את השגיאה שאין לך הרשאה **(550 5.7.13),** הפעל את הפקודה הבאה [ב- Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` לדוגמה, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני לתיקיה ציבורית זו, הוסף את הגישה CreateItems למשתמש אנונימי. לדוגמה, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
