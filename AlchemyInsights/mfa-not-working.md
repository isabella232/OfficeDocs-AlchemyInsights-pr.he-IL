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
# <a name="issues-with-mfa"></a><span data-ttu-id="32873-102">בעיות עם משרד התואר</span><span class="sxs-lookup"><span data-stu-id="32873-102">Issues with MFA</span></span>
<span data-ttu-id="32873-103">יש כמה דברים לבדוק אם למשתמשים אין אפשרות להתחבר באמצעות אימות מרובה גורמים (משרד החוץ)</span><span class="sxs-lookup"><span data-stu-id="32873-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="32873-104">המשתמש המושפע יכול להיות חסום בפורטל הספריה הפעילה.</span><span class="sxs-lookup"><span data-stu-id="32873-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="32873-105">אם זהו המקרה, נסיונות האימות עבור משתמש ספציפי זה יידחו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="32873-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="32873-106">נא בצע את הפעולות במאמר זה כדי לבטל את חסימתן.</span><span class="sxs-lookup"><span data-stu-id="32873-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="32873-107">אם הסרת חסימה של המשתמש לא עזרה או המשתמש לא נחסם באפשרותך לנסות לאפס את משרד התואר הטוב ביותר עבור המשתמש והם יעבור את תהליך ההרשמה שוב.</span><span class="sxs-lookup"><span data-stu-id="32873-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="32873-108">נא בצע את השלבים הבאים במאמר זה.</span><span class="sxs-lookup"><span data-stu-id="32873-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="32873-109">אם זו הפעם הראשונה בה הפכת את משרד החוץ לזמין והמשתמשים אינם יכולים להתחבר ללקוחות שאינם דפדפנים כגון Outlook, סקייפ, וכו ', אולי ADAL (ספריית אימות Active Directory) אינה זמינה במנוי O365 שלך.</span><span class="sxs-lookup"><span data-stu-id="32873-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="32873-110">במקרה זה יהיה עליך להתחבר ל-Exchange Online Powershell ולהפעיל יישומון cmdlet זה:  *Set-OAuth2ClientProfileEnabled הארגונית: $true*</span><span class="sxs-lookup"><span data-stu-id="32873-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>