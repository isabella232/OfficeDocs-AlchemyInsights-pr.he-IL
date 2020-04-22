---
title: תיקון בעיות העברת דואר אלקטרוני לתיקיות ציבוריות התומכות בדואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716353"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>תיקון בעיות העברת דואר אלקטרוני לתיקיות ציבוריות התומכות בדואר

אם שולחים חיצוניים אינם יכולים לשלוח הודעות לתיקיות הציבוריות המותאמות לדואר שלך, והשולחים מקבלים את השגיאה: **לא נמצא (550 5.4.1)**, ודא שתחום הדואר האלקטרוני עבור התיקיה הציבורית מוגדר כתחום ממסר פנימי במקום תחום סמכותי:

1. פתח את [מרכז הניהול של Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. עבור אל \> **קבוצות מחשבים מקובלות**של **זרימת דואר** , בחר את התחום המקובל ולאחר מכן לחץ על **עריכה**.

3. בדף המאפיינים שנפתח, אם סוג התחום מוגדר **כסמכותי**, שנה את הערך **לממסר פנימי** ולאחר מכן לחץ על **שמור**.

אם שולחים חיצוניים מקבלים את השגיאה **שאין לך הרשאה (550 5.7.13)**, הפעל את הפקודה הבאה ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous``Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`. לדוגמא

כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני לתיקיה ציבורית זו, הוסף את הגישה של CreateItems ישירות למשתמש אנונימי. `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`. לדוגמא
