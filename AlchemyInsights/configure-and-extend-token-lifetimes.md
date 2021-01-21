---
title: קביעת תצורה והארכה של אורך חיים של אסימונים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916827"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="f9684-102">קביעת תצורה והארכה של אורך חיים של אסימונים</span><span class="sxs-lookup"><span data-stu-id="f9684-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="f9684-103">באפשרותך לציין את אורך החיים של האסימון access, SAML או ID שהונפק על-ידי פלטפורמת הזהות של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f9684-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="f9684-104">באפשרותך להגדיר אורך חיים של אסימונים עבור כל היישומים בארגון שלך, עבור יישום רב-דייר (מרובה ארגונים), או עבור מנהל שירות ספציפי בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="f9684-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="f9684-105">לקבלת מידע נוסף, קרא [אורך חיים של אסימונים הניתנים להגדרה](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="f9684-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="f9684-106">לקבלת דוגמאות, קרא [דוגמאות לאופן הגדרת אורך חיים של אסימונים](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="f9684-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="f9684-107">כדי ללמוד כיצד להגדיר את משך החיים והתאימות של אסימון בתכלת Active Directory B2C (תכלת AD B2C), ראה [קביעת תצורה של אסימונים בתכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="f9684-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="f9684-108">המאמר [קביעת התצורה של אופן הפעולה של הפעלה ב-תכלת Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) מתאר את שיטות הכניסה היחידה (SSO) המשמשות ב-תכלת AD B2C ועוזר לך לבחור את שיטת ה-sso המתאימה ביותר בעת קביעת התצורה של המדיניות שלך.</span><span class="sxs-lookup"><span data-stu-id="f9684-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="f9684-109">**כמה זמן יימשך אסימונים? לכמה זמן הם תקפים?**</span><span class="sxs-lookup"><span data-stu-id="f9684-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="f9684-110">אורך חיים של אסימונים הוא שעה והמשך הזמן של ההפעלה הוא 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="f9684-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="f9684-111">משמעות הדבר היא שאם לא בוצעו בקשות ב-24 שעות, יהיה עליך להיכנס שוב לפני בקשת אסימון חדש.</span><span class="sxs-lookup"><span data-stu-id="f9684-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="f9684-112">לאחר 30 במאי 2020, אף דייר חדש לא יוכל להשתמש במדיניות לכל החיים של אסימונים הניתנים להגדרה כדי לקבוע את התצורה של אסימוני הפעלה ורענון.</span><span class="sxs-lookup"><span data-stu-id="f9684-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="f9684-113">התבטלות יקרה תוך מספר חודשים לאחר מכן, כלומר, נפסיק לכבד הפעלה קיימת ונרענן משטרת אסימונים.</span><span class="sxs-lookup"><span data-stu-id="f9684-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="f9684-114">עדיין ניתן לקבוע את התצורה של אורך חיים של אסימון גישה לאחר תבטלות.</span><span class="sxs-lookup"><span data-stu-id="f9684-114">You can still configure access token lifetimes after the deprecation.</span></span>






