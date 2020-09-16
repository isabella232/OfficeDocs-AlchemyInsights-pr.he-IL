---
title: תיקון שגיאת 0x8004de40 ב-OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745131"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>תיקון שגיאת 0x8004de40 ב-OneDrive

אם אתה מקבל שגיאת 0x8004de40 עם OneDrive:

- הפעל מחדש את המחשב המושפע בעת חיבור לתחום מדריך הכתובות שלך ב-Acitve.
- אם אתחול מחדש אינו פותר את הבעיה, הצטרף למכשיר והצטרף אליו מחדש מתכלת לספירה. 

**הערה**: עליך להיות ברשת החברה שלך בעת ביצוע שלבים אלה. אל תבצע שלבים אלה כאשר אינך מצליח להתחבר לתשתית הארגונית שלך (לדוגמה, בעת נסיעה). 

- פתח שורת פקודה מוגבהת. 
- כדי לפתוח שורת פקודה מוגבהת, לחץ על **התחל**, לחץ באמצעות לחצן העכבר הימני על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.
- הקלד *dsregcmd/leave* והקש **Enter**.
- כאשר תסיים, הקלד *dsregcmd/join* והקש **Enter**.
- כאשר תסיים, סגור את שורת הפקודה.
- אתחל מחדש את המחשב והיכנס ל-OneDrive.