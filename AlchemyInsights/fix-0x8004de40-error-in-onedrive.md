---
title: תקן את השגיאה 0x8004de40 ב- OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525060"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>תקן את השגיאה 0x8004de40 ב- OneDrive

אם מתקבלת שגיאה 0x8004de40 עם OneDrive:

- אתחל מחדש את המחשב המושפע במצב מחובר לתחום הספריה Acitve שלך.
- אם אתחול מחדש לא פותר את הבעיה, הצטרפות לקבוצת והצטרף המכשיר הפרסומת תכלת הרקיע. 

**הערה**: עליך לנהוג ברשת של החברה שלך בעת ביצוע שלבים אלה. אל תבצע את הפעולות הבאות כאשר אינם יכולים להתחבר תשתית החברה שלך (לדוגמה, בעת נסיעה). 

- פתח שורת פקודה בעלת הרשאות מלאות. 
- כדי לפתוח שורת פקודה בעלת הרשאות מלאות, לחץ על - **התחלה**, לחץ לחיצה ימנית על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.
- הקלד *dsregcmd /leave* והקש **Enter**.
- בסיום, הקלד *dsregcmd /join* והקש **Enter**.
- בסיום, לסגור את שורת הפקודה.
- אתחל מחדש את המחשב ולאחר מכן היכנס לתוך OneDrive.