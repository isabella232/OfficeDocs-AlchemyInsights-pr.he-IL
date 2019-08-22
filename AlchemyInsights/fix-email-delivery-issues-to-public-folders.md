---
title: לפתור בעיות מסירה של דואר אלקטרוני לתיקיות ציבוריות התומכים בדואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525108"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>לפתור בעיות מסירה של דואר אלקטרוני לתיקיות ציבוריות התומכים בדואר

אם שולחים חיצוניים אין אפשרות לשלוח הודעות אל התיקיות הציבוריות שלך התומכים בדואר, ולקבל שולחים השגיאה: **לא נמצא (550 5.4.1)**, ודא לתחום דואר אלקטרוני עבור התיקיה הציבורית נקבעה כתחום ממסר פנימי של במקום קבוצת מחשבים מוסמכים:

1. פתח את [מרכז הניהול של Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. עבור אל **זרימת דואר** \> **תחומים שהתקבלו**, בחר את התחום המקובל, ולאחר מכן לחץ על **ערוך**.

3. מאפייני דף זה נפתח, אם לסוג תחום מוגדר **Authoritative**, שנה את הערך ל **ממסר פנימי** ולאחר מכן לחץ על **שמור**.

אם שולחים חיצוניים מקבל שגיאה **שאין לך הרשאה (550 5.7.13)**, הפעל את הפקודה הבאה ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`לדוגמה, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני אל תיקיה ציבורית זו, הוסף את הגישה CreateItems מימין משתמש אנונימי. לדוגמה, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
