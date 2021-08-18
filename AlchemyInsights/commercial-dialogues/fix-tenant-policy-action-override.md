---
title: תיקון מדיניות דיירים (עקיפת פעולה)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326798"
---
# <a name="fix-tenant-policy-action-override"></a>תיקון מדיניות דיירים (עקיפת פעולה)

אחד ממדיניות האנטי-דואר זבל שלך השפיע על הודעה זו. כדי לסקור את פריטי המדיניות, בצע את השלבים הבאים:

1. בפורטל Microsoft 365 Defender ב- , עבור אל מדיניות שיתוף פעולה & דואר אלקטרוני & כללים מדיניות איומים נגד דואר <https://security.microsoft.com/>  \>  \>  \>  זבל **במקטע מדיניות.**

   כדי לעבור ישירות לדף **מדיניות למניעת דואר זבל,** השתמש <https://security.microsoft.com/antispam> ב- .

2. בדף מדיניות **למניעת** דואר זבל, בחר את המדיניות על-ידי לחיצה על  שם המדיניות (**הקלד** הוא מדיניות מותאמת אישית למניעת דואר זבל או **שם** הוא מדיניות כניסה למניעת דואר **זבל (ברירת מחדל).**
3. בתפריט נשלף של הפרטים שמופיע, **בחר ערוך** פעולות **במקטע** פעולות.
4. במקטע פעולות **הודעה,** סקור את פסקי הדין עבור דואר זבל **,**  דואר זבל בביטחון **גבוה,** דיוג **ו** דיוג בביטחון גבוה כדי לראות אם אחד מהערכים הבאים נבחר:
   - **הוספת X-header**
   - **שורת הנושא 'הכנה' עם טקסט**
   - **ניתוב מחדש של הודעה לכתובת דואר אלקטרוני**
   - **מחיקת הודעה**
   - **ללא פעולה**

   ייתכן שההגדרות הרגילות **שהוחלו** על כל Exchange Online Protection השפיעו על ההודעה.

לקבלת מידע נוסף, ראה [קביעת תצורה של מדיניות למניעת דואר זבל ב- EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
