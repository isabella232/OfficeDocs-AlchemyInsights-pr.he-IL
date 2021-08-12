---
title: בעיות ביצועים- SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911843"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint או OneDrive איטיים, לא נגישים או לא זמינים עבור משתמשים מרובים

SharePoint או OneDrive עשויים להיות איטיים, לא נגישים או לא זמינים, או עשויים להציג שגיאות של שירות לא זמין או 503, מכמה סיבות:
  
- אם אתר SharePoint או OneDrive איטי או מושהה עבור משתמשים מרובים, ייתכן שיש בעיית שירות זמנית שבה המשתמשים נתקלים בעיכובים לסירוגין או בשגיאות ניווט בעת גישה לאתרי SharePoint או OneDrive תוכן. בדוק את [לוח המחוונים של](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) תקינות השירות כדי לראות אם הארגון שלך מושפע.
  
- המשתמשים עשויים לקבל שרת *503* הוא שגיאה לא פנויה בעת ניסיון לנווט אל SharePoint או OneDrive שלך. שגיאה זו עשויה להיגרם על-ידי ויסות SharePoint השירות. SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ומהימנות אופטימליים של שירות SharePoint Online. ויסות מגביל את מספר פעולות המשתמש או מספר השיחות בו-זמנית (לפי script או קוד) כדי למנוע שימוש מופרז במשאבים. לקבלת מידע נוסף אודות ויסות, ראה [הימנעות מ ויסות או חסימה ב- SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- אם אתה נתקל בביצועים איטיים עם **אתר** **או** דף SharePoint קלאסיים או מודרניים, השתמש בכלי 'אבחון [דפים'](https://aka.ms/perftool) כדי לנתח את הדפים.
  
- אם אתה עדיין נתקל בביצועים איטיים כלליים, עיין במשאבים בחלק התחתון של מאמר זה: [מבוא לכוונון ביצועים עבור SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  