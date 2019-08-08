---
title: החלף את אתר הבסיס הקלאסי עם אתר מודרני
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245993"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>החלף את אתר הבסיס הקלאסי עם אתר מודרני

אם הסביבה שלך הוגדר לפני 2019 באפריל, באפשרותך לשנות את אתר הבסיס שלך לאתר מודרני באמצעות Microsoft PowerShell:

- אם יש לך אתר אחר שברצונך להשתמש בשם אתר הבסיס שלך, באפשרותך להחליף אתר (swap) הבסיס איתו. 
    - השתמש [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) להחליף את המיקום של אתר עם אתר אחר בעת אחסון בארכיון של האתר המקורי. אפשרות זו זמינה עבור אתר הצוות (לא מחובר לקבוצה) ואתר תקשורת. 

- יכולות נוספות שהוכנסו בקרוב אשר יאפשר לך לשמור באמצעות התוכן באתר, אך להמיר אתר קיים לאתר תקשורת. 
>[!Important]
>אלה יכולות לפרוס בהדרגה. המשך לבדיקת מרכז הודעת Office 365 עבור עדכונים. 

## <a name="known-issues-with-swapping-sites"></a>בעיות מוכרות עם החלפה של אתרים

- אתר היעד עלול להחזיר הודעת שגיאה "לא נמצא" (HTTP 404) עבור פרק זמן קצר.
- התוכן יהיה עליך להיות recrawled כדי לעדכן אינדקס החיפוש. אין לא נדרש שלב ידנית - הדבר יבוצע באופן אוטומטי.
- דבר תלוי סטטי"קישורים (כגון קבצי סינכרון קובץ ו- OneNote) יהיה עליך לתקן באופן ידני.
- אם אתר המקור היה אתר חדשות של הארגון, לעדכן את כתובת ה-URL.קבל רשימה של כל אתרי חדשות של הארגון.
- אתרים שרת הפרוייקט, ייתכן שתצטרך להיות מאומתים כדי לוודא שהן עדיין משויכת כראוי.





