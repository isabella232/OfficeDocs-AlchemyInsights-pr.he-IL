---
title: אתר מודרני כמקום הבסיס
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327603"
---
# <a name="modern-site-as-root-site"></a>אתר מודרני כמקום בסיס

התחלנו להציג תכונה חדשה שתאפשר לך להחליף את אתר הבסיס הקלאסי [שלך באתר מודרני.](https://docs.microsoft.com/sharepoint/modern-root-site) השתמש [ב- Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר תוך אחסון האתר המקורי בארכיון. זמין הן עבור אתר הצוות (לא מחובר לקבוצה) וגם עבור אתר תקשורת.

**חשוב**: אל תמחק את אתר הבסיס הקלאסי שלך כדי ליצור אתר תקשורת מודרני. פעולה זו אינה נתמכת על-ידי Microsoft. מחיקת אתר הבסיס תגרום לכל אתרי SharePoint בארגון שלך להיות בלתי נגישים לכל המשתמשים, עד שתשחזר את האתר או תיצור אתר חדש באותה כתובת URL. אנו נקשר תכונה זו דרך מרכז ההודעות. עליך לצפות שהתכונה תהיה מופעלת בתוך הדייר שלך בקרוב.

## <a name="known-issues-with-swapping-sites"></a>בעיות ידועות עם החלפת אתרים
- אתר היעד עשוי להחזיר שגיאת "לא נמצא" (HTTP 404) במשך פרק זמן קצר.
- יהיה צורך ליצור מחדש תוכן כדי לעדכן את אינדקס החיפוש. לא נדרש כאן שלב ידני, פעולה זו ת בוצע באופן אוטומטי.
- כל דבר התלוי בקישורים "סטטיים" (כגון סינכרון קבצים OneNote קבצים) יתוקן באופן ידני.
- Project ייתכן שיהיה צורך לאמת אתרי שרת כדי לוודא שהם עדיין משויכים כראוי. 
