---
title: בעיות בנושא תואר בכיר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755132"
---
# <a name="issues-with-azure-mfa"></a>בעיות עם משרד החוץ של התכלת
יש כמה דברים שכדאי לבדוק אם משתמשים אינם יכולים להיכנס באמצעות אימות רב-גורמי.

1. ייתכן שהמשתמש המושפע נחסם בפורטל תכלת Active Directory. אם זהו המצב, מתבצעת דחייה אוטומטית של נסיונות אימות עבור משתמש ספציפי זה. [בצע את השלבים המפורטים במאמר זה כדי לבטל את חסימתם.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. אם ביטול החסימה של המשתמש לא הועיל או אם המשתמש לא נחסם, באפשרותך לנסות לאפס את ה-it עבור המשתמש והם יעברו את תהליך ההרשמה שוב. [בצע את השלבים המפורטים במאמר זה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

אם זו הפעם הראשונה שאתה משתמש ב-university והמשתמשים שלך אינם יכולים להיכנס ללקוחות שאינם לקוחות בדפדפנים כגון Outlook, Skype, etc, אולי ADAL (ספריית האימות של Active Directory) אינה זמינה במנוי O365 שלך. במקרה זה, יהיה עליך להתחבר ל-Exchange Online Powershell ולהפעיל את ה-cmdlet הבא:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*