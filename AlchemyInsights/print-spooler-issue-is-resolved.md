---
title: בעיית מנגנון ההדפסה ברקע נפתרה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911339"
---
# <a name="print-spooler-issue-is-resolved"></a>בעיית מנגנון ההדפסה ברקע נפתרה

אם המכשיר שלך עודכן ב- Windows 10 **גירסת Build מס' 19041.329** של מערכת ההפעלה, ייתכן שצפית בבעיה שבה מדפסות מסוימות לא מצליחות להדפיס.   מנגנון ההדפסה ברקע עשוי להשליך שגיאה או לסגור באופן בלתי צפוי בעת ניסיון להדפיס, ולא מגיע פלט מהדפסת המושפעת. בעיה זו נפתרה בגליון Build  **מס' 19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**חקירה מתמשכת**

הקובץ Local Security Security Authority Subsystem Service (LSASS) (**Isass.exe**) עשוי להיכשל במכשירים מסוימים באמצעות הודעת השגיאה "תהליך מערכת קריטי, C:\WINDOWS\system32\Isass.exe, נכשל עם קוד המצב c00000008. כעת יש להפעיל מחדש את המחשב".  **Microsoft עובדת על פתרון והיא תספק עדכון במהדורה עתידית.**

לקבלת מידע נוסף, עיין בבעיות [מוכרות Windows 10 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).