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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545168"
---
# <a name="issues-with-mfa"></a>בעיות עם משרד התואר
יש כמה דברים לבדוק אם למשתמשים אין אפשרות להתחבר באמצעות אימות מרובה גורמים (משרד החוץ)

1. המשתמש המושפע יכול להיות חסום בפורטל הספריה הפעילה. אם זהו המקרה, נסיונות האימות עבור משתמש ספציפי זה יידחו באופן אוטומטי. [נא בצע את הפעולות במאמר זה כדי לבטל את חסימתן.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. אם הסרת חסימה של המשתמש לא עזרה או המשתמש לא נחסם באפשרותך לנסות לאפס את משרד התואר הטוב ביותר עבור המשתמש והם יעבור את תהליך ההרשמה שוב. [נא בצע את השלבים הבאים במאמר זה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

אם זו הפעם הראשונה בה הפכת את משרד החוץ לזמין והמשתמשים אינם יכולים להתחבר ללקוחות שאינם דפדפנים כגון Outlook, סקייפ, וכו ', אולי ADAL (ספריית אימות Active Directory) אינה זמינה במנוי O365 שלך. במקרה זה יהיה עליך להתחבר ל-Exchange Online Powershell ולהפעיל יישומון cmdlet זה:  *Set-OAuth2ClientProfileEnabled הארגונית: $true*