---
title: בעיה בהצטרפות לוירטואלית
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885210"
---
# <a name="issue-joining-vms"></a>בעיה בהצטרפות לוירטואלית

כדי לפתור בעיות המתרחשות בעת ניסיון להצטרף ל-וירטואלית, בצע את השלבים הבאים:

1. נסה להיכנס באמצעות תבנית **UPN** (לדוגמה, ' joeuser@contoso.com ') במקום בתבנית **SAMAccountName** (' CONTOSO\joeuser ').
2. ודא שהפעלת סינכרון סיסמאות בהתאם לשלבים *המתוארים במדריך תחילת* העבודה.
3. ודא שחשבון המשתמש המושפע אינו חשבון חיצוני בדייר תכלת לספירה. משתמשים חיצוניים אינם יכולים להיכנס לתחום המנוהל מאחר ששירותי התחום של תכלת AD אינם כוללים אישורים עבור חשבונות משתמשים אלה.
4. אם חשבון המשתמש המושפע הוא חשבון משתמש בענן בלבד, ודא שהמשתמשים החליפו את הסיסמה שלהם לאחר הפעלת שירותים בתחום התכלת של AD. שלב זה גורם לפעולות ה-hash של האישורים הדרושים עבור שירותי התחום של תכלת AD ליצירה.
5. אם חשבונות המשתמשים המושפעים מסונכרנים מתוך מדריך כתובות מקומי, ודא שתצורת ההפצה המומלצת של התחברות התכלת של התכלת הוגדרה לביצוע סינכרון מלא.
6. אם הבעיות נמשכות לאחר אישור שלב 4, הפעל את הפקודות הבאות מתוך מחשב הסינכרון:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.