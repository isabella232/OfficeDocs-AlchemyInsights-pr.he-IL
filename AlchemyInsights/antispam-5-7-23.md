---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932170"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>פתרון בעיות במסירת דואר אלקטרוני עבור קוד שגיאה 5.7.23

אמת את רשומת ה- DNS של SPF עבור התחום שלך ב- SPF או בודק רשומות DNS הזמין לציבור באינטרנט.

ודא שההודעה היוצאת לא זוהתה כנת זבל על-ידי Microsoft וניתב דרך מאגר [מסירת סיכונים גבוהים](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). הודעות ב' מאגר מסירה בסיכון גבוה' לא יעברו בדיקת SPF, ולכן לא יתקבלו על-ידי ארגון הדואר האלקטרוני המשמש כיעד.

אם הבעיה נמשכת, ייתכן שתצטרך לפנות למנהל של מארח הדואר שאתה מנסה לשלוח לו דואר אלקטרוני. רשום לעצמך את השגיאה החיצונית המפורטת הזמינה בה הודעת ההקפצת. ייתכן שהתמיכה של Microsoft לא תוכל לסייע עוד יותר.
