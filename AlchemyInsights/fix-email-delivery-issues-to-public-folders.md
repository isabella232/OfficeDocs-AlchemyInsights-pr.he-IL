---
title: פתרון בעיות במסירת דואר אלקטרוני לתיקיות ציבוריות המותאמות לדואר
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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677929"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>פתרון בעיות במסירת דואר אלקטרוני לתיקיות ציבוריות המותאמות לדואר

אם שולחים חיצוניים אינם יכולים לשלוח הודעות לתיקיות ציבוריות המותאמות לדואר שלך, והשולחים מקבלים את השגיאה: **לא ניתן למצוא אותו (550 5.4.1)**, לוודא שתחום הדואר האלקטרוני של התיקיה הציבורית מוגדר כתחום ממסר פנימי במקום תחום סמכותי:

1. פתח את [מרכז הניהול של Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. עבור אל **Mail flow** \> **תחומים מקובלים**של זרימת דואר, בחר את התחום המקובל ולאחר מכן לחץ על **ערוך**.

3. בעמוד המאפיינים שנפתח, אם סוג התחום מוגדר **כסמכותי**, שנה את הערך **לממסר פנימי** ולאחר מכן לחץ על **שמור**.

אם שולחים חיצוניים מקבלים את השגיאה **שאין לך הרשאה (550 5.7.13)**, השתמש בפקודה הבאה ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) כדי לראות את ההרשאות עבור משתמשים אנונימיים בתיקיה הציבורית:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` לדוגמה, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

כדי לאפשר למשתמשים חיצוניים לשלוח דואר אלקטרוני לתיקיה ציבורית זו, הוסף את הגישה CreateItems ישירות למשתמש בעילום שם. לדוגמה, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
