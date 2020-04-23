---
title: תקן את השגיאה 0x8004de40 ב OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716029"
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