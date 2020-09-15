---
title: אתר מודרני בתור אתר הבסיס
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666871"
---
# <a name="modern-site-as-root-site"></a>אתר מודרני כאתר בסיס

התחלנו להציג תכונה חדשה שתאפשר לך [להחליף את אתר הבסיס הקלאסי של האתר באמצעות אתר מודרני](https://docs.microsoft.com/sharepoint/modern-root-site). השתמש באפשרות [הפעל את SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בזמן אחסון האתר המקורי. זמין עבור שני אתרי הצוות (שאינם מחוברים לקבוצה) ולאתר תקשורת.

>[!Important]
> אל תמחק את אתר הבסיס הקלאסי כדי ליצור אתר תקשורת מודרני. פעולה זו אינה נתמכת על-ידי Microsoft. מחיקת אתר הבסיס תגרום לכל אתרי SharePoint בארגון שלך לא להיות נגישים לכל המשתמשים, עד שתשחזר את האתר או תיצור אתר חדש באותו כתובת URL. אנו ניצור תקשורת של תכונה זו דרך מרכז ההודעות. אתה אמור לצפות שהתכונה מופעלת בדייר שלך בקרוב.

## <a name="known-issues-with-swapping-sites"></a>בעיות ידועות בנושא החלפת אתרים
- אתר היעד עשוי להחזיר שגיאת "לא נמצא" (HTTP 404) לפרק זמן קצר.
- יהיה צורך לסרוק משוב תוכן כדי לעדכן את אינדקס החיפוש. אין צורך בשלב ידני כאן, פעולה זו תתבצע באופן אוטומטי.
- כל דבר תלוי בקישורים סטטיים (כגון קבצי סינכרון וקבצי OneNote) יצטרכו לתקן אותו באופן ידני.
- ייתכן שיהיה עליך לאמת את אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי. 
