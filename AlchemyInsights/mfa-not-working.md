---
title: בעיות ב- MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098603"
---
# <a name="issues-with-azure-mfa"></a>בעיות ב- Azure MFA
יש כמה דברים שיש לבדוק אם משתמשים אינם יכולים להיכנס באמצעות אימות רב-גורמי (MFA)

1. המשתמש המושפע עשוי להיחסם בפורטל Azure Active Directory. במקרה זה, ניסיונות האימות עבור משתמש ספציפי זה נדחתה באופן אוטומטי. [בצע את השלבים המפורטים במאמר זה כדי לבטל את החסימה שלהם.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. אם ביטול החסימה של המשתמש לא עזר או שהמשתמש לא נחסם, באפשרותך לנסות לאפס את MFA עבור המשתמש והוא י לעבור את תהליך ההרשמה שוב. [בצע את השלבים המפורטים במאמר זה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

אם זו הפעם הראשונה שהפיצת את MFA והמשתמשים שלך אינם יכולים להיכנס ללקוחות שאינם דפדפנים, כגון Outlook, Skype וכן הלאה, ייתכן ש- ADAL (ספריית אימות Active Directory) אינו זמין במנוי O365 שלך. במקרה זה יהיה עליך להתחבר ל- Exchange Online Powershell ולהפעיל cmdlet זה: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*