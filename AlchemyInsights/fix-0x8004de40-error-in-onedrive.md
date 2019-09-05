---
title: תקן את השגיאה 0x8004de40 ב OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755849"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>תקן את השגיאה 0x8004de40 ב OneDrive

אם אתה מקבל שגיאת 0x8004de40 עם OneDrive:

- אתחל מחדש את המחשב המושפע בעת ההתחברות לקבוצת המחשבים של ספריית Acitve.
- אם אתחול מחדש אינו מתקן את הבעיה, בטל את הצירוף והצטרף מחדש להתקן מתכלת AD. 

**הערה**: עליך להיות ברשת החברה שלך בעת ביצוע שלבים אלה. אל תבצע שלבים אלה כאשר אינך מצליח להתחבר לתשתית הארגונית (לדוגמה, בעת נסיעה). 

- פתח שורת פקודה עם הרשאות מלאות. 
- כדי לפתוח שורת פקודה מוגבה, לחץ על **התחל**, לחץ לחיצה ימנית על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.
- הקלד *dsregcmd/השאר* והקש **Enter**.
- בעת השלמתו, הקלד *dsregcmd/join* והקש **Enter**.
- לאחר השלמתו, סגור את שורת הפקודה.
- אתחל את המחשב והיכנס למערכת OneDrive.