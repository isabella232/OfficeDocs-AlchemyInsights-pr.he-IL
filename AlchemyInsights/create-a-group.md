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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816357"
---
# <a name="create-a-group"></a>יצירת קבוצה

נושא זה מתאר יצירת קבוצה.

**הרשאה ליצירת קבוצה**

ודא שאתה מורשה ליצור קבוצה חדשה. מנהלי מערכת כלליים יכולים להפוך יצירת קבוצה ללא זמינה בפורטל Azure או Access ה- Panel. ייתכן שתצטרך מנהל מערכת כדי ליצור את הקבוצה החדשה בשבילך, או כדי להעניק לך הרשאות מתאימות.

**ניהול הרשאות יצירת קבוצה**

1. מנהלי מערכת כלליים יכולים לנהל הרשאות יצירת קבוצות (מסיבות הקשורות לאבטחה) או קבוצות Office 365 שנוצרו בפורטל Azure או בלוח Access, על-ידי בחירה באפשרות "משתמשים יכולים ליצור קבוצות אבטחה בפורטלים של Azure" או "משתמשים יכולים ליצור קבוצות Office 365 בפורטלים של Azure" בכל הקבוצות  >  **הכלליות (הגדרות).**
2. באפשרותך גם להגביל יצירת קבוצה כדי לבחור קבוצת משתמשים אם יש לך רשיון Azure Active Directory P1 Premium.

**הפיכת הודעת ברוך הבא ללא זמין עבור חברי הקבוצה החדשים של Office 365**

ניתן לבטל את הודעת הפתיחה שנשלחת למשתמשים שנוספו לקבוצות Office 365 על-ידי הגדרת **UnifiedGroupWelcomeMessageEnabled** ל- False ב- Powershell. קבל מידע על הגדרה זו [כאן](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

