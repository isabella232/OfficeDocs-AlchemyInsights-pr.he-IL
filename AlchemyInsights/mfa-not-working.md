---
title: בעיות עם משרד התואר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768838"
---
# <a name="issues-with-azure-mfa"></a>בעיות עם התכלת
יש כמה דברים לבדוק אם למשתמשים אין אפשרות להיכנס למערכת באמצעות אימות מרובה גורמים (משרד החוץ)

1. המשתמש המושפע יכול להיות חסום בפורטל הספריה הפעילה. אם זהו המקרה, נסיונות האימות עבור משתמש ספציפי זה יידחו באופן אוטומטי. [נא בצע את הפעולות במאמר זה כדי לבטל את חסימתן.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. אם הסרת חסימה של המשתמש לא עזרה או המשתמש לא נחסם באפשרותך לנסות לאפס את משרד התואר הטוב ביותר עבור המשתמש והם יעבור את תהליך ההרשמה שוב. [נא בצע את השלבים הבאים במאמר זה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

אם זו הפעם הראשונה בה הפכת את משרד החוץ לזמין והמשתמשים אינם יכולים להתחבר ללקוחות שאינם דפדפנים כגון Outlook, סקייפ, וכו ', אולי ADAL (ספריית אימות Active Directory) אינה זמינה במנוי O365 שלך. במקרה זה יהיה עליך להתחבר ל-Exchange Online Powershell ולהפעיל יישומון cmdlet זה:  *Set-OAuth2ClientProfileEnabled הארגונית: $true*