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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768838"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="e6d39-102">בעיות עם התכלת</span><span class="sxs-lookup"><span data-stu-id="e6d39-102">Issues with Azure MFA</span></span>
<span data-ttu-id="e6d39-103">יש כמה דברים לבדוק אם למשתמשים אין אפשרות להיכנס למערכת באמצעות אימות מרובה גורמים (משרד החוץ)</span><span class="sxs-lookup"><span data-stu-id="e6d39-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="e6d39-104">המשתמש המושפע יכול להיות חסום בפורטל הספריה הפעילה.</span><span class="sxs-lookup"><span data-stu-id="e6d39-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="e6d39-105">אם זהו המקרה, נסיונות האימות עבור משתמש ספציפי זה יידחו באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="e6d39-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="e6d39-106">נא בצע את הפעולות במאמר זה כדי לבטל את חסימתן.</span><span class="sxs-lookup"><span data-stu-id="e6d39-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="e6d39-107">אם הסרת חסימה של המשתמש לא עזרה או המשתמש לא נחסם באפשרותך לנסות לאפס את משרד התואר הטוב ביותר עבור המשתמש והם יעבור את תהליך ההרשמה שוב.</span><span class="sxs-lookup"><span data-stu-id="e6d39-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="e6d39-108">נא בצע את השלבים הבאים במאמר זה.</span><span class="sxs-lookup"><span data-stu-id="e6d39-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="e6d39-109">אם זו הפעם הראשונה בה הפכת את משרד החוץ לזמין והמשתמשים אינם יכולים להתחבר ללקוחות שאינם דפדפנים כגון Outlook, סקייפ, וכו ', אולי ADAL (ספריית אימות Active Directory) אינה זמינה במנוי O365 שלך.</span><span class="sxs-lookup"><span data-stu-id="e6d39-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="e6d39-110">במקרה זה יהיה עליך להתחבר ל-Exchange Online Powershell ולהפעיל יישומון cmdlet זה:  *Set-OAuth2ClientProfileEnabled הארגונית: $true*</span><span class="sxs-lookup"><span data-stu-id="e6d39-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>