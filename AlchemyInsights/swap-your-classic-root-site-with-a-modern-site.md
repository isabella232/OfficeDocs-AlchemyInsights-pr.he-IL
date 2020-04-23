---
title: החלף את אתר השורש הקלאסי שלך עם אתר מודרני
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741545"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>החלף את אתר השורש הקלאסי שלך עם אתר מודרני

אם הסביבה שלך הוגדרה לפני אפריל 2019, באפשרותך לשנות את אתר השורש שלך לאתר מודרני באמצעות Microsoft PowerShell:

- אם יש לך אתר שונה בו ברצונך להשתמש כאתר הבסיס שלך, באפשרותך להחליף [(להחליף) את אתר השורש](https://docs.microsoft.com/sharepoint/modern-root-site) בו. 
    - השתמש באפשרות [הפעל-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בעת אחסון האתר המקורי בארכיון. זמין עבור האתר הקבוצתי (לא מחובר לקבוצה) ולאתר תקשורת. 

- יכולות נוספות יוצגו בקרוב שיאפשרו לך להמשיך להשתמש בתוכן באתר, אך להמיר את האתר הקיים לאתר תקשורת. 
>[!Important]
>יכולות אלה יוגלגלו בהדרגה. המשך לבדוק את מרכז ההודעות לקבלת עדכונים. 

## <a name="known-issues-with-swapping-sites"></a>בעיות ידועות עם החלפת אתרים

- אתר היעד עשוי להחזיר שגיאה "לא נמצאה" (HTTP 404) למשך פרק זמן קצר.
- התוכן צריך להיות מעודכן כדי לעדכן את אינדקס החיפוש. אין צורך בצעד ידני-זה ייעשה באופן אוטומטי.
- כל דבר התלוי בקישורים "סטטיים" (כגון קבצי סינכרון קבצים ו-OneNote) יהיה צורך לתקן באופן ידני.
- אם אתר המקור היה אתר חדשות ארגוני, עדכן את כתובת ה-URL.תשיגי רשימה של כל. אתרי החדשות האירגוניים
- ייתכן שיהיה צורך באימות של אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי.
