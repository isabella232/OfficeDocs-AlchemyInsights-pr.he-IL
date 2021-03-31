---
title: תכניות בסיסיות של EndPoint Manager - Security
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440885"
---
# <a name="endpoint-manager---security-baselines"></a>תכניות בסיסיות של EndPoint Manager - Security

תוכניות אבטחה בסיסיות הן קבוצות של הגדרות Windows מוגדרות מראש שעוזרות לך להחיל את הגדרות האבטחה שצוותי אבטחה רלוונטיים ממליצים להם. התוכניות הבסיסיות הללו פתוחות להתאמות שמאפשרות למסור רק את ההגדרות והערכים הרצויים. למידע נוסף על תוכניות אבטחה בסיסיות ראה [שימוש בתוכניות אבטחה בסיסיות לקביעת תצורה של מכשירי Windows 10 ב- Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

נכון לעכשיו, יש תוכניות בסיסיות למוצרים הבאים:

- הגדרות אבטחה של Windows MDM
- Microsoft Defender ל- EndPoint Security
- Microsoft Edge

כל אחת מהתוכניות הבסיסיות מתעדכנת מעת לעת ומופצת בגרסאות מצטברות. בכל גרסה מתווספות או נגרעות הגדרות מהגרסה הקודמת כדי להבטיח שהתוכנית הבסיסית עומדת בדרישות הקו המנחה העדכני. מסוף תכניות האבטחה הבסיסיות ב- Endpoint Security מאפשר השוואה בין גרסאות שונות בכך שהוא מאפשר לראות את ההבדלים בין גרסה אחת לשנייה.

ראו הדרכה על השינויים היעילים ביותר לכל גרסה של תכנית בסיסית כאן [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

לאחר התקנת תוכנית אבטחה בסיסית באפשרותך לנטר את מצב ההתקנה ולבחון מחדש הגדרות של מכשיר אחר מכשיר.

**שים לב:** ייתכן שיחלפו עד 24 שעות עד הופעתם של נתוני דיווח על תוכניות בסיסיות מהתקנה הראשונית במכשיר. בעדכונים נוספים, עד שש שעות. 

הסיבה הנפוצה ביותר לאי החלה של הגדרת תוכנית בסיסית היא שאותה הגדרה נמצאת בשימוש בפרופיל אחר. אפשר לבדוק את התרחיש בכל מכשיר על-ידי בחירתו בצומת 'מצב מכשיר' בפרופיל ה- Security Baseline. ראה מידע מפורט כאן [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).