---
title: בעיה ב- AAD התחברות תקינות
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923753"
---
# <a name="problem-with-aad-connect-health"></a>בעיה ב- AAD התחברות תקינות

- ודא שאתה מורשה לבצע את הפעולה. למנהלי מערכת כלליים יש גישה כברירת מחדל. בנוסף, באפשרותך להשתמש בפקד [מבוסס Access כדי להקצות](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) הרשאת רישום למשתתף.
- ודא שנקודות הקצה הדרושות זמינות ולא נחסמות עקב חומת אש. לקבלת פרטים, [ראה דרישות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- הרישום עלול להיכשל עקב תקשורת יוצאת הנבדקת ב- SSL על-ידי שכבת הרשת.
- ודא שאומתת את הגדרות ההודעות עבור Azure AD התחברות תקינות. סקור את ההגדרה שלך. מדריך [זה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) יכול לעזור לך להבין כיצד לקבוע את התצורה של הגדרות ההודעות עבור Azure AD התחברות הודעות תקינות.
- כדי ללמוד עוד אודות סינכרון AAD התחברות תקינות ואופן הדוח, ראה [סינכרון ברמת האובייקטים הדוח](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

כדי לפתור בעיות בהתראות AAD התחברות תקינות, פעל בהתאם למדריך לפתרון בעיות עבור [התראות רעננות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) של נתוני AAD התחברות ולשאלות נפוצות, ראה שאלות נפוצות [בנושא התקנה התחברות תקינות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
