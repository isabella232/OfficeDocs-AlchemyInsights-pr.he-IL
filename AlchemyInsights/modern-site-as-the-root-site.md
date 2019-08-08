---
title: אתר מודרניים כמו אתר הבסיס
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232716"
---
# <a name="modern-site-as-root-site"></a>אתר מודרני כאתר הבסיס

אנו שהתחילו כדי ההשקה תכונה חדשה שתאפשר לך להחליף את אתר הבסיס אתר קלאסי עם אתר מודרני. השתמש [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) להחליף את המיקום של אתר עם אתר אחר בעת אחסון בארכיון של האתר המקורי. אפשרות זו זמינה עבור אתר הצוות (לא מחובר לקבוצה) ואתר תקשורת. 

>[!Important]
> אל תמחק את אתר הבסיס קלאסית ליצירת אתר תקשורת מודרניים. פעולה זו אינה נתמכת על-ידי Microsoft. מחיקת אתר הבסיס יבצע כל אתרי SharePoint בארגון שלך נגישים לכל המשתמשים, עד לשחזר את האתר או ליצור אתר חדש בכתובת ה-URL זהה. אנו לקיים תקשורת תכונה זו דרך מרכז ההודעה. עליך לצפות את התכונה כדי להיות מופעלת בדיירים שלך בקרוב.

## <a name="known-issues-with-swapping-sites"></a>בעיות מוכרות עם החלפה של אתרים
- אתר היעד עלול להחזיר הודעת שגיאה "לא נמצא" (HTTP 404) עבור פרק זמן קצר.
- התוכן יהיה עליך להיות recrawled כדי לעדכן אינדקס החיפוש. אין שלב ידני לא נדרש כאן, הדבר יבוצע באופן אוטומטי.
- דבר תלוי סטטי"קישורים (כגון קבצי סינכרון קובץ ו- OneNote) יהיה עליך לתקן באופן ידני.
- אתרים שרת הפרוייקט, ייתכן שתצטרך להיות מאומתים כדי לוודא שהן עדיין משויכת כראוי. 
