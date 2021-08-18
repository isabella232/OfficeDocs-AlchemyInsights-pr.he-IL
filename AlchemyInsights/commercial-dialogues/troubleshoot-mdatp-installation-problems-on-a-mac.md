---
title: פתרון בעיות בהתקנת MDATP ב- Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091033"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>פתרון בעיות בהתקנת MDATP ב- Mac

אם ההתקנה הידני נכשלת, **העמוד סיכום** של אשף ההתקנה מציג את השגיאה הבאה:

"אירעה שגיאה במהלך ההתקנה. תוכנית ההתקנה נתקלה בשגיאה שגרמה לכשל בהתקנה. פנה ליצרן התוכנה לקבלת סיוע."

עבור פריסות MDM, הדף מציג גם כשל התקנה כללי.

למרות שאנו לא מציגים שגיאות מדויקות למשתמשי קצה, אנו שומרים קובץ יומן רישום עם התקדמות ההתקנה, **ב- /Library/Logs/Microsoft/mdatp/install.log.** כל הפעלת התקנה מצרף לקובץ יומן רישום זה. כדי ליצור פלט של הפעלת ההתקנה האחרונה בלבד, השתמש `sed` ב- .

לקבלת מידע נוסף, ראה [פתרון בעיות התקנה עבור Microsoft Defender ATP עבור Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
