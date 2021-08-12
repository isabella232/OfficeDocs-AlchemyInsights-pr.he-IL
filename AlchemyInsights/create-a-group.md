---
title: יצירת קבוצה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929306"
---
# <a name="create-a-group"></a>יצירת קבוצה

נושא זה מתאר יצירת קבוצה.

**הרשאה ליצירת קבוצה**

ודא שאתה מורשה ליצור קבוצה חדשה. מנהלי מערכת כלליים יכולים להפוך יצירת קבוצה ללא זמינה בפורטל Azure או Access ה- Panel. ייתכן שתצטרך מנהל מערכת כדי ליצור את הקבוצה החדשה בשבילך, או כדי להעניק לך הרשאות מתאימות.

**ניהול הרשאות יצירת קבוצה**

1. מנהלי מערכת כלליים יכולים לנהל הרשאות יצירת קבוצות (מסיבות הקשורות לאבטחה) או קבוצות Office 365 שנוצרו בפורטל Azure או בלוח Access, על-ידי בחירה באפשרות "משתמשים יכולים ליצור קבוצות אבטחה בפורטלים של Azure" או "משתמשים יכולים ליצור קבוצות Office 365 בפורטלים של Azure" בכל הקבוצות  >  **כלליות (הגדרות).**
2. באפשרותך גם להגביל יצירת קבוצה כדי לבחור קבוצת משתמשים אם יש לך רשיון Azure Active Directory P1 Premium רישוי.

**הפיכת הודעת ברוך הבא ללא Office 365 חדשים**

ניתן לבטל את הודעת הפתיחה שנשלחת למשתמשים שנוספו לקבוצות Office 365 על-ידי הגדרת **UnifiedGroupWelcomeMessageEnabled** ל- False ב- Powershell. קבל מידע על הגדרה זו [כאן](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

