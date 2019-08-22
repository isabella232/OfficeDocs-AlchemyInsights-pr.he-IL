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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545168"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="97061-102">בעיות עם MFA</span><span class="sxs-lookup"><span data-stu-id="97061-102">Issues with MFA</span></span>
<span data-ttu-id="97061-103">ישנם מספר דברים כדי לבדוק אם למשתמשים אין אפשרות להיכנס למערכת באמצעות אימות מגורמים רבים (MFA)</span><span class="sxs-lookup"><span data-stu-id="97061-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="97061-104">המשתמש המושפע עשויות להיחסם בפורטל מדריך הכתובות הפעיל תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="97061-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="97061-105">אם זהו המקרה, של ניסיונות אימות עבור אשר משתמש ספציפי באופן אוטומטי תידחה.</span><span class="sxs-lookup"><span data-stu-id="97061-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="97061-106">נא בצע את הפעולות המתוארות במאמר זה כדי להסיר מעליהם את החסימה.</span><span class="sxs-lookup"><span data-stu-id="97061-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="97061-107">אם ביטול חסימה של המשתמש לא סייע או המשתמש אינה חסומה שבאפשרותך לנסות כדי לאפס MFA עבור המשתמש והם יעברו דרך תהליך הרשמה שוב.</span><span class="sxs-lookup"><span data-stu-id="97061-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="97061-108">נא בצע את הפעולות המתוארות במאמר זה.</span><span class="sxs-lookup"><span data-stu-id="97061-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="97061-109">אם זו הפעם הראשונה MFA זמין והמשתמשים שלך אינך מצליח להיכנס ללקוחות שאינם דפדפנים כגון Outlook, Skype וכו ', אולי ADAL (ספריית אימות הספריה הפעילה) אינה זמינה במנוי שלך O365.</span><span class="sxs-lookup"><span data-stu-id="97061-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="97061-110">במקרה זה יהיה עליך להתחבר ל- Exchange Online Powershell ולהפעיל cmdlet זה:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="97061-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>