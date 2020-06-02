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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506444"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>תקן בעיות משלוח דוא ל עבור קוד שגיאה 5.7.23

אמת את רשומת ה-SPF DNS עבור התחום שלך בבודק רשומות מסוג SPF או DNS זמין לציבור באינטרנט.

ודא שההודעה היוצאת לא זוהתה כהודעת זבל על-ידי Microsoft ונותבה באמצעות [מאגר המסירה לסיכון גבוה](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). הודעות במאגר האספקה של הסיכון הגבוה לא יעברו בדיקות SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המהווה יעד.

אם הבעיה נמשכת, ייתכן שיהיה עליך לפנות למנהל המארח של הדואר שאליו אתה מנסה לשלוח דואר אלקטרוני. רשום את השגיאה החיצונית המפורטת הזמינה בהודעת הניתור. ייתכן שהתמיכה של Microsoft לא תוכל לסייע בהמשך.
