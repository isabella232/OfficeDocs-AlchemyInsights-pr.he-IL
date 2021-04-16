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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="74c4a-102">בעיות ב- Azure MFA</span><span class="sxs-lookup"><span data-stu-id="74c4a-102">Issues with Azure MFA</span></span>
<span data-ttu-id="74c4a-103">יש כמה דברים שיש לבדוק אם משתמשים אינם יכולים להיכנס באמצעות אימות רב-גורמי (MFA)</span><span class="sxs-lookup"><span data-stu-id="74c4a-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="74c4a-104">המשתמש המושפע עשוי להיחסם בפורטל Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="74c4a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="74c4a-105">במקרה זה, ניסיונות האימות עבור משתמש ספציפי זה נדחתה באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="74c4a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="74c4a-106">בצע את השלבים המפורטים במאמר זה כדי לבטל את החסימה שלהם.</span><span class="sxs-lookup"><span data-stu-id="74c4a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="74c4a-107">אם ביטול החסימה של המשתמש לא עזר או שהמשתמש לא נחסם, באפשרותך לנסות לאפס את MFA עבור המשתמש והוא י לעבור את תהליך ההרשמה שוב.</span><span class="sxs-lookup"><span data-stu-id="74c4a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="74c4a-108">בצע את השלבים המפורטים במאמר זה.</span><span class="sxs-lookup"><span data-stu-id="74c4a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="74c4a-109">אם זו הפעם הראשונה שהפינית את MFA לזמין והמשתמשים שלך אינם יכולים להיכנס ללקוחות שאינם דפדפנים, כגון Outlook, Skype וכדומה, ייתכן ש- ADAL (ספריית אימות Active Directory) אינה זמינה במנוי O365 שלך.</span><span class="sxs-lookup"><span data-stu-id="74c4a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="74c4a-110">במקרה זה תצטרך להתחבר ל- Exchange Online Powershell ולהפעיל cmdlet זה:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="74c4a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>