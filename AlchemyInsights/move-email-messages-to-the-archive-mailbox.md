---
title: העברת הודעות דואר אלקטרוני בתיבת הדואר של ארכיון
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660381"
---
בעיות אחסון בארכיון של פריטים בתיבת הדואר של ארכיון. ודא שביצעת את השלבים הבאים:
  
1. ודא כי **לאחסן בארכיון דואר** הפכה לזמינה. אם לא, בצע את הפעולות במאמר [זה](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) כדי להפעיל את תיבת הדואר של ארכיון. 
    
2. במרכז הניהול של Exchange, בחר **תגיות השמירה** תחת **ניהול תאימות**, ליצור **תגית שמירה** עם פעולת **העבר לארכיון** המכיל את **גיל השמירה**הרצויה.
    
3. במרכז הניהול של Exchange, בחר **מדיניות שמירה**, ליצור **מדיניות שמירה** ולהוסיף תגית השמירה שלך **להעביר לארכיון** מדיניות זו. 
    
4. [הקצאת מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) תיבת דואר של משתמש מסוים. באותה המדיניות יוחלו על **ראשי** וגם את תיבת הדואר של **ארכיון** . 
    
תיבת הדואר של המשתמש אמורה להיות מדיניות ארכיון כדי להעביר פריטים בתיבת הדואר של ארכיון. ייתכן שיהיה עליך לכפות את מנוהל תיקיה המסייע (MFA) כדי להפעיל, להחיל את ההגדרות החדשות לתיבת הדואר של המשתמש. הפעל את הפקודה הבאה בעת [מחובר EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את ניהול מסייע התיקיות עבור תיבת דואר מסוימת: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

מעוניין במידע נוסף אודות הגדרת מדיניות אחסון בארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה של תיבות דואר](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

