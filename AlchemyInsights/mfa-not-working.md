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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="1eacc-102">בעיות עם משרד החוץ של התכלת</span><span class="sxs-lookup"><span data-stu-id="1eacc-102">Issues with Azure MFA</span></span>
<span data-ttu-id="1eacc-103">יש כמה דברים שכדאי לבדוק אם משתמשים אינם יכולים להיכנס באמצעות אימות רב-גורמי.</span><span class="sxs-lookup"><span data-stu-id="1eacc-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="1eacc-104">ייתכן שהמשתמש המושפע נחסם בפורטל תכלת Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1eacc-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="1eacc-105">אם זהו המצב, מתבצעת דחייה אוטומטית של נסיונות אימות עבור משתמש ספציפי זה.</span><span class="sxs-lookup"><span data-stu-id="1eacc-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="1eacc-106">בצע את השלבים המפורטים במאמר זה כדי לבטל את חסימתם.</span><span class="sxs-lookup"><span data-stu-id="1eacc-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="1eacc-107">אם ביטול החסימה של המשתמש לא הועיל או אם המשתמש לא נחסם, באפשרותך לנסות לאפס את ה-it עבור המשתמש והם יעברו את תהליך ההרשמה שוב.</span><span class="sxs-lookup"><span data-stu-id="1eacc-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="1eacc-108">בצע את השלבים המפורטים במאמר זה.</span><span class="sxs-lookup"><span data-stu-id="1eacc-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="1eacc-109">אם זו הפעם הראשונה שאתה משתמש ב-university והמשתמשים שלך אינם יכולים להיכנס ללקוחות שאינם לקוחות בדפדפנים כגון Outlook, Skype, etc, אולי ADAL (ספריית האימות של Active Directory) אינה זמינה במנוי O365 שלך.</span><span class="sxs-lookup"><span data-stu-id="1eacc-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="1eacc-110">במקרה זה, יהיה עליך להתחבר ל-Exchange Online Powershell ולהפעיל את ה-cmdlet הבא:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="1eacc-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>