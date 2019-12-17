---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068404"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint או OneDrive איטי, לא נגיש או לא זמין עבור משתמשים מרובים

SharePoint או OneDrive עשויים להיות איטיים, לא נגישים או לא זמינים, או שהשירות יציג שירות שאינו זמין או 503 שגיאות, ממספר סיבות:
  
- אם אתר SharePoint או OneDrive שלך איטי או מתעכב עבור משתמשים מרובים, ייתכן שקיימת בעיית שירות זמנית שבה משתמשים חווים עיכובים לסירוגין או שגיאות ניווט בעת גישה לאתרי SharePoint או לתוכן OneDrive. בדוק את [לוח המחוונים של תקינות השירות](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק אם הארגון שלך מושפע.
  
- משתמשים עלולים לקבל *שרת 503 הוא* שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או onedrive. שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint. SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online. האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים. לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- אם אתה נתקל בביצועים איטיים עם אתר או דף SharePoint **קלאסי** או **מודרני** , נצל את [כלי אבחון העמוד](https://aka.ms/perftool) כדי לנתח את הדפים.
  
- אם אתה עדיין נתקל בביצועים איטיים כלליים, עיין במשאבים בחלק התחתון של מאמר זה: [מבוא לכיוונון ביצועים עבור SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  