---
title: החלפת אתר הבסיס הקלאסי שלך באתר מודרני
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316141"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>החלפת אתר הבסיס הקלאסי שלך באתר מודרני

אם הסביבה שלך הוגדרה לפני אפריל 2019, באפשרותך לשנות את אתר הבסיס שלך לאתר מודרני באמצעות Microsoft PowerShell:

- אם יש לך אתר אחר שברצונך להשתמש בו כ אתר הבסיס שלך, באפשרותך להחליף [(להחליף) את אתר הבסיס](https://docs.microsoft.com/sharepoint/modern-root-site) בו. 
    - השתמש [ב- Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר תוך אחסון האתר המקורי בארכיון. זמין הן עבור אתר הצוות (לא מחובר לקבוצה) וגם עבור אתר תקשורת. 

- יכולות נוספות יוצגו בקרוב שיאפשרו לך להמשיך להשתמש בתוכן באתר, אך להמיר את האתר הקיים לאתר תקשורת. 

**חשוב**: יכולות אלה יגולגלו בהדרגה. המשך לבדוק אם קיימים עדכונים במרכז ההודעות. 

## <a name="known-issues-with-swapping-sites"></a>בעיות ידועות עם החלפת אתרים

- אתר היעד עשוי להחזיר שגיאת "לא נמצא" (HTTP 404) במשך פרק זמן קצר.
- יהיה צורך ליצור מחדש תוכן כדי לעדכן את אינדקס החיפוש. לא נדרש שלב ידני - פעולה זו ת בוצע באופן אוטומטי.
- כל דבר התלוי בקישורים "סטטיים" (כגון סינכרון קבצים OneNote קבצים) יתוקן באופן ידני.
- אם אתר המקור היה אתר חדשות ארגוני, עדכן את כתובת ה- URL. קבל רשימה של כל אתרי החדשות הארגוניים.
- Project ייתכן שיהיה צורך לאמת אתרי שרת כדי לוודא שהם עדיין משויכים כראוי.
