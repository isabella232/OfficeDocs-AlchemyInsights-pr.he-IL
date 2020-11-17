---
title: יצירת קבוצה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088903"
---
# <a name="create-a-group"></a>יצירת קבוצה

נושא זה מתאר יצירת קבוצה.

**הרשאה ליצירת קבוצה**

ודא שאתה מורשה ליצור קבוצה חדשה. מנהלי מערכת כלליים יכולים להפוך את יצירת הקבוצה ללא זמינה בלוח תכלת או בלוח הגישה. ייתכן שתזדקק למנהל מערכת כדי ליצור את הקבוצה החדשה עבורך, או כדי להעניק לך הרשאות מתאימות.

**ניהול הרשאות יצירת קבוצה**

1. מנהלי מערכת כלליים יכולים לנהל הרשאות יצירת קבוצה (למטרות הקשורות לאבטחה) או קבוצות של Office 365 שנוצרו בפורטל תכלת או ב-Access, על-ידי בחירה "משתמשים יכולים ליצור קבוצות אבטחה בפורטלים של תכלת" או "משתמשים יכולים ליצור קבוצות של office 365 בפורטלים של תכלת" בכל **הקבוצות**  >  **כללי (**
2. באפשרותך גם להגביל את יצירת הקבוצה כדי לבחור קבוצת משתמשים אם יש לך רשיון תכלת של Active Directory P1 Premium.

**הפיכת הודעת הפתיחה ללא זמינה עבור חברים בקבוצה חדשה של Office 365**

ניתן להפוך את הודעת הפתיחה למשתמשים שנוספו לקבוצות של Office 365 לבלתי זמינה על-ידי הגדרת **UnifiedGroupWelcomeMessageEnabled** ל-False ב-Powershell. קבל מידע על הגדרה זו [כאן](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

