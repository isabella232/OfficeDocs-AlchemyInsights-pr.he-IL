---
title: בעיות ביצועים-SharePoint או OneDrive
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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771902"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint או OneDrive איטיים, לא נגישים או שאינם זמינים עבור משתמשים מרובים

SharePoint או OneDrive עשויים להיות איטיים, בלתי נגישים או שאינם זמינים, או עשויים להציג שגיאות שאינן זמינות או 503, מכמה סיבות:
  
- אם האתר שלך ב-SharePoint או ב-OneDrive מתעכב או מעוכב עבור משתמשים מרובים, ייתכן שקיימת בעיה זמנית בשירות שבו משתמשים חווים עיכובים רציפים או שגיאות ניווט בעת גישה לאתרי SharePoint או לתוכן OneDrive. בדוק את [לוח המחוונים של תקינות השירות](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק אם הארגון שלך מושפע.
  
- משתמשים עשויים לקבל שגיאה של *503 server עמוסה* בעת ניסיון לנווט לאתרי SharePoint או OneDrive. שגיאה זו עשויה להיגרם כתוצאה מוויסות בשירות SharePoint. SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ומהימנות אופטימליים של שירות SharePoint Online. ויסות מגביל את מספר פעולות המשתמש או מספר השיחות בו-זמנית (לפי script או קוד) כדי למנוע שימוש מופרז במשאבים. לקבלת מידע נוסף אודות ויסות, ראה [הימנעות מקבלת מצערת או חסומה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- אם אתה נתקל בביצועים איטיים באמצעות אתר או אתר SharePoint **קלאסי** או **מודרני** , השתמש [בכלי אבחון העמוד](https://aka.ms/perftool) כדי לנתח את העמודים.
  
- אם אתה עדיין נתקל בביצועים איטיים כלליים, עיין במשאבים בחלק התחתון של מאמר זה: [מבוא לכוונון ביצועים עבור SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  