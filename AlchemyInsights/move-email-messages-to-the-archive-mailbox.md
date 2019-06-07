---
title: העברת הודעות דואר אלקטרוני בתיבת הדואר של ארכיון
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762366"
---
# <a name="move-email-to-the-archive-mailbox"></a>העבר דואר אלקטרוני בתיבת הדואר של ארכיון
 
1. ודא כי **לאחסן בארכיון דואר** הפכה לזמינה. אם לא, בצע את הפעולות במאמר [זה](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) כדי להפעיל את תיבת הדואר של ארכיון.

2. כדי לאחסן בארכיון הודעות באופן אוטומטי תיבת הדואר של ארכיון, יש להגדיר תג שמירה עם פעולת **העבר לאחסן בארכיון** כדי **להחיל באופן אוטומטי על תג תיבת הדואר כולה (ברירת המחדל)**. השתמש בשלבים כאן כדי ליצור את התג: [תג ברירת מחדל של ארכיון](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. לאחר מכן, הוסף את תג **ארכיון** למדיניות השמירה שלך. במרכז הניהול של Exchange, בחר **מדיניות שמירה** > להוסיף **לקליפ תג ארכיון** > מדיניות **שמירה**. 
    
4. כעת [להקצות מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) תיבת דואר של משתמש מסוים. באותה המדיניות יוחלו על **ראשי** וגם את תיבת הדואר של **ארכיון** . 
    
ייתכן שיהיה עליך לכפות את מנוהל תיקיה המסייע (MFA) כדי להפעיל, להחיל את ההגדרות החדשות לתיבת הדואר של המשתמש. הפעל את הפקודה הבאה בעת [מחובר EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את ניהול מסייע התיקיות עבור תיבת דואר מסוימת: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

לקבלת מידע נוסף אודות הגדרת מדיניות אחסון בארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה של תיבות דואר](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

