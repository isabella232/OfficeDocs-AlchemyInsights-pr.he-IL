---
title: בעיות עם MFA
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250166"
---
# <a name="issues-with-mfa"></a>בעיות עם MFA
ישנם מספר דברים כדי לבדוק אם למשתמשים אין אפשרות להיכנס למערכת באמצעות אימות מגורמים רבים (MFA)

1. המשתמש המושפע עשויות להיחסם בפורטל מדריך הכתובות הפעיל תכלת הרקיע. אם זהו המקרה, של ניסיונות אימות עבור אשר משתמש ספציפי באופן אוטומטי תידחה. [נא בצע את הפעולות המתוארות במאמר זה כדי להסיר מעליהם את החסימה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. אם ביטול חסימה של המשתמש לא סייע או המשתמש אינה חסומה שבאפשרותך לנסות כדי לאפס MFA עבור המשתמש והם יעברו דרך תהליך הרשמה שוב. [נא בצע את הפעולות המתוארות במאמר זה.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

אם זו הפעם הראשונה MFA זמין והמשתמשים שלך אינך מצליח להיכנס ללקוחות שאינם דפדפנים כגון Outlook, Skype וכו ', אולי ADAL (ספריית אימות הספריה הפעילה) אינה זמינה במנוי שלך O365. במקרה זה יהיה עליך להתחבר ל- Exchange Online Powershell ולהפעיל cmdlet זה:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*