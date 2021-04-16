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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810485"
---
# <a name="issues-with-azure-mfa"></a>בעיות ב- Azure MFA
יש כמה דברים שיש לבדוק אם משתמשים אינם יכולים להיכנס באמצעות אימות רב-גורמי (MFA)

1. המשתמש המושפע עשוי להיחסם בפורטל Azure Active Directory. במקרה זה, ניסיונות האימות עבור משתמש ספציפי זה נדחתה באופן אוטומטי. [בצע את השלבים המפורטים במאמר זה כדי לבטל את החסימה שלהם.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. אם ביטול החסימה של המשתמש לא עזר או שהמשתמש לא נחסם, באפשרותך לנסות לאפס את MFA עבור המשתמש והוא י לעבור את תהליך ההרשמה שוב. [בצע את השלבים המפורטים במאמר זה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

אם זו הפעם הראשונה שהפינית את MFA לזמין והמשתמשים שלך אינם יכולים להיכנס ללקוחות שאינם דפדפנים, כגון Outlook, Skype וכדומה, ייתכן ש- ADAL (ספריית אימות Active Directory) אינה זמינה במנוי O365 שלך. במקרה זה תצטרך להתחבר ל- Exchange Online Powershell ולהפעיל cmdlet זה:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*