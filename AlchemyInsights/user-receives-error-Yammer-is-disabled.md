---
title: המשתמש מקבל שגיאה AADSTS7000112 Yammer אינו זמין
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198058"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>המשתמש מקבל שגיאה AADSTS7000112 Yammer אינו זמין

אם אתה מקבל את השגיאה "AADSTS7000112: יישום" 00000005-0000-0ff1-ce00-000000000000 ' (Yammer) אינו זמין ", קיימת בעיה עם מנהל השירות בתוך התכלת. ייתכן שמנהל המערכת ביטל את מנהל השירות כדי לחסום את הגישה ליאממר.

השבתת מנהל השירות אינה מומלצת ויכולה לגרום לבעיות נוספות. לקבלת מידע נוסף אודות הגישה הנתמכת לחסימת גישת המשתמש ליאממר, ראה [ביטול גישת yammer עבור משתמשי Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

כדי לתקן בעיה זו בפורטל התכלת ולשחזר את גישת המשתמש ליאממר:

1.  פתח את הדף ' מדריך כחול פעיל ' ובחר **יישומים ארגוניים** תחת **ניהול** בחלונית הניווט השמאלית.
3.  הקלד **Office 365 Yammer** בתיבת החיפוש, ובחר את שם היישום כדי לפתוח את ההגדרות.
4.  בחר **מאפיינים** תחת **ניהול** בחלונית הניווט השמאלית.
5.  האם להגדיר את הערך **הזמין עבור משתמשים להיכנס?** **ככן**ולאחר מכן בחר **שמור**.
6.  . היכנס ליאממר שוב . אולי תצטרך לנקות את העוגיות

לחלופין, הפעל פקודות PowerShell כדי להגדיר את הערך. לקבלת מידע נוסף, ראה ["מצטערים, אך אנו מתקשים לחתום על השגיאה" בעת לחיצה על האריח Yammer ב-Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 