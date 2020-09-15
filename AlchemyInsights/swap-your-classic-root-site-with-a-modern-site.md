---
title: החלפת אתר הבסיס הקלאסי באמצעות אתר מודרני
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691180"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>החלפת אתר הבסיס הקלאסי באמצעות אתר מודרני

אם הסביבה שלך הוגדרה לפני אפריל 2019, באפשרותך לשנות את אתר הבסיס לאתר מודרני באמצעות Microsoft PowerShell:

- אם יש לך אתר אחר שבו ברצונך להשתמש כאתר הבסיס שלך, באפשרותך להחליף [(להחליף) את אתר הבסיס](https://docs.microsoft.com/sharepoint/modern-root-site) שלו. 
    - השתמש באפשרות [הפעל את SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בזמן אחסון האתר המקורי. זמין עבור שני אתרי הצוות (שאינם מחוברים לקבוצה) ולאתר תקשורת. 

- יכולות נוספות יוצגו בקרוב שיאפשרו לך להמשיך להשתמש בתוכן באתר, אך להמיר את האתר הקיים לאתר תקשורת. 
>[!Important]
>יכולות אלה יסוכמו בהדרגה. המשך לבדוק אם קיימים עדכונים במרכז ההודעות. 

## <a name="known-issues-with-swapping-sites"></a>בעיות ידועות בנושא החלפת אתרים

- אתר היעד עשוי להחזיר שגיאת "לא נמצא" (HTTP 404) לפרק זמן קצר.
- יהיה צורך לסרוק משוב תוכן כדי לעדכן את אינדקס החיפוש. אין צורך בשלב ידני-פעולה זו תתבצע באופן אוטומטי.
- כל דבר תלוי בקישורים סטטיים (כגון קבצי סינכרון וקבצי OneNote) יצטרכו לתקן אותו באופן ידני.
- אם אתר המקור היה אתר חדשות ארגוני, עדכן את כתובת ה-URL.קבל רשימה של כל אתרי החדשות הארגוניים.
- ייתכן שיהיה עליך לאמת את אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי.
