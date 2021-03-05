---
title: בעיה עם האפשרות ' התחבר לתקינות '
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482067"
---
# <a name="problem-with-aad-connect-health"></a>בעיה עם האפשרות ' התחבר לתקינות '

- ודא שאתה מורשה לבצע את הפעולה. למנהלי מערכת כלליים יש גישה כברירת מחדל. בנוסף, באפשרותך להשתמש [בבקרת גישה מבוססת תפקידים](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) כדי להקצות הרשאת רישום למשתתף.
- ודא שנקודות הקצה הנדרשות זמינות, ולא נחסמות עקב חומת האש. לקבלת פרטים, ראה [דרישות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- הרישום עשוי להיכשל עקב תקשורת יוצאת הנתונה לפיקוח SSL על-ידי שכבת הרשת.
- ודא שאימתת את הגדרות ההודעה עבור בריאות הקישור תכלת לספירה. עיין בהגדרה. [מדריך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) זה יכול לעזור לך להבין כיצד לקבוע את התצורה של הגדרות ההודעה עבור הודעות בריאות של תכלת לספירה.
- לקבלת מידע נוסף אודות דוח הסינכרון של התקינות של החיבור הרפואי של ה-עמ ואופן ההורדה שלו, ראה [דוח סינכרון ברמת האובייקט](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

כדי לפתור בעיות בחיבור של התראות תקינות, בצע [את מדריך פתרון הבעיות עבור הצגת התראות טריות של נתוני תקינות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ולגבי שאלות נפוצות, ראה האפשרות [המשותפת לגבי התקנת שאלות של התקנת תקינות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
