---
title: אתר מודרני כאתר השורש
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713792"
---
# <a name="modern-site-as-root-site"></a>אתר מודרני כאתר שורש

התחלנו לפריסה תכונה חדשה שתאפשר לך [להחליף את האתר הקלאסי שלך בסיס האתר עם אתר מודרני](https://docs.microsoft.com/sharepoint/modern-root-site). השתמש באפשרות [הפעל-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בעת אחסון האתר המקורי בארכיון. זמין עבור האתר הקבוצתי (לא מחובר לקבוצה) ולאתר תקשורת.

>[!Important]
> אל תמחק את אתר השורש הקלאסי שלך כדי ליצור אתר תקשורת מודרני. הדבר אינו נתמך על-ידי Microsoft. מחיקת אתר הבסיס תהפוך את כל אתרי SharePoint בארגון שלך לנגישים לכל המשתמשים, עד שתשחזר את האתר או תיצור אתר חדש באותו כתובת URL. אנו מתקשרים עם תכונה זו באמצעות מרכז ההודעות. אתה צריך לצפות את התכונה להיות מופעלת הדייר שלך בקרוב.

## <a name="known-issues-with-swapping-sites"></a>בעיות ידועות עם החלפת אתרים
- אתר היעד עשוי להחזיר שגיאה "לא נמצאה" (HTTP 404) למשך פרק זמן קצר.
- התוכן צריך להיות מעודכן כדי לעדכן את אינדקס החיפוש. אין צורך בצעד ידני, זה ייעשה באופן אוטומטי.
- כל דבר התלוי בקישורים "סטטיים" (כגון קבצי סינכרון קבצים ו-OneNote) יהיה צורך לתקן באופן ידני.
- ייתכן שיהיה צורך באימות של אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי. 
