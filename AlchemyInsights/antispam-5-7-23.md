---
title: ספאם-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717326"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>פתרון בעיות במסירת דואר אלקטרוני עבור קוד שגיאה 5.7.23

אמת את רשומת ה-SPF DNS עבור התחום שלך בבודק רשומות SPF או DNS הזמין באופן ציבורי באינטרנט.

ודא שההודעה היוצאת לא זוהתה כהודעת זבל על-ידי Microsoft והמנותבת באמצעות [בריכת המסירה הגבוהה לסיכון](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). הודעות בבריכת המסירה בסיכון גבוה לא יעברו בדיקות SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המשמש כיעד.

אם הבעיה נמשכת, ייתכן שיהיה עליך לפנות למנהל המארח של הדואר שאליו אתה מנסה לשלוח דואר אלקטרוני. רשום לעצמך את השגיאה החיצונית המפורטת הזמינה בהודעת הניתור. ייתכן שהתמיכה של Microsoft לא תוכל לסייע עוד.
