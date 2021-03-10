---
title: פתרון בעיות בהתקנת MDATP ב-Mac
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694278"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>פתרון בעיות בהתקנת MDATP ב-Mac

אם ההתקנה הידנית נכשלת, דף **הסיכום** של אשף ההתקנה מציג את השגיאה הבאה:

"אירעה שגיאה במהלך ההתקנה. תוכנית ההתקנה נתקלה בשגיאה שגרמה להתקנה להיכשל. פנה ליצרן התוכנה לקבלת סיוע.

עבור פריסות MDM, הדף מציג כשל כללי בהתקנה.

למרות שאין באפשרותנו להציג שגיאות מדויקות למשתמשי הקצה, אנו שועטים את קובץ יומן הרישום עם התקדמות ההתקנה, ב- **/Library/Logs/Microsoft/mdatp/install.log**. כל הפעלת התקנה מצורפת לקובץ יומן רישום זה. כדי להפיק פלט של הפעלת ההתקנה האחרונה בלבד, השתמש באפשרות `sed` .

לקבלת מידע נוסף, ראה [פתרון בעיות התקנה עבור Microsoft DEFENDER ATP עבור Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
