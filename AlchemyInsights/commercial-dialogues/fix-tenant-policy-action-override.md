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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896076"
---
# <a name="fix-tenant-policy-action-override"></a>תיקון מדיניות דיירים (עקיפת פעולה)

אחד ממדיניות האנטי-דואר זבל שלך השפיע על הודעה זו. כדי לסקור את פריטי המדיניות, בצע את השלבים הבאים:

1. בפורטל Microsoft 365 Defender, עבור אל מדיניות שיתוף פעולה & דואר אלקטרוני & מדיניות איומים של כללים נגד דואר <https://security.microsoft.com/>  \>  \>  \>  זבל **במקטע מדיניות.**

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
