---
title: פתרון בעיות בדואר אלקטרוני
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569141"
---
# <a name="troubleshooting-events-from-email"></a>פתרון בעיות בדואר אלקטרוני

1. ודא שהתכונה מאופשרת עבור תיבת הדואר: מערכת <mailbox>

2. לאחר מכן, הביטו ביומני הרישום של ' אירועי דואר אלקטרוני ' <mailbox>

3. ביומני ' אירועים מתוך דואר אלקטרוני ', מצא את מזהה ה-Internetהודעה התואם לפריט בתיבת הדואר.  

4. תוצאת האמון קובעת אם הפריט נוסף או לא. אירועים יתווספו רק אם האמון בציון = "מהימן".

תוצאת האמון נקבעת על-ידי המאפיינים SPF, Dkim או Dkim, הנמצאים בכותרת ההודעה.

כדי להציג מאפיינים אלה:

**שולחן העבודה Outlook**

- פתח את הפריט
- קובץ-_ Gt_ מאפיינים-_ Gt_ כותרות אינטרנט

או

**מעגל שפיר**

- ניווט לפריט בתיבת הדואר הנכנס
- חפש PR_TRANSPORT_MESSAGE_HEADERS_W

מאפיינים אלה נקבעים ונרשמים במהלך הובלה וניתוב. לפתרון בעיות נוסף, ייתכן שיהיה עליך להמשיך בטיפול בתמיכת תעבורה אודות הכשלים ב-SPF, DKIM ו-. או DKIM.