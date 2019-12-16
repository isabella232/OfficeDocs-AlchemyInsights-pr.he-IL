---
title: תקן את השגיאה 0x8004de40 ב OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052038"
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