---
title: אנטי ספאם-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682156"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>תקן בעיות משלוח דוא ל עבור קוד שגיאה 5.7.23

אמת את רשומת ה-SPF DNS עבור התחום שלך בבודק רשומות מסוג SPF או DNS זמין לציבור באינטרנט.

ודא שההודעה היוצאת לא זוהתה כהודעת זבל על-ידי Office 365 ונותבה דרך [מאגר האספקה הגבוה](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). הודעות במאגר האספקה של הסיכון הגבוה לא יעברו בדיקות SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המהווה יעד.

אם הבעיה נמשכת, ייתכן שיהיה עליך לפנות למנהל המארח של הדואר שאליו אתה מנסה לשלוח דואר אלקטרוני. רשום את השגיאה החיצונית המפורטת הזמינה בהודעת הניתור.  ייתכן שהתמיכה ב-Office 365 לא תוכל לסייע בהמשך.