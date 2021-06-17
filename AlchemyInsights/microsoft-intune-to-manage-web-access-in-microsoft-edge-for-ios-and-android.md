---
title: שימוש ב- Microsoft Intune לניהול גישה לאינטרנט ב- Microsoft Edge עבור iOS ו- Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989674"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="da619-102">שימוש ב- Microsoft Intune לניהול גישה לאינטרנט ב- Microsoft Edge עבור iOS ו- Android</span><span class="sxs-lookup"><span data-stu-id="da619-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="da619-103">Microsoft Edge עבור iOS ו- Android מאפשר למשתמש לגלוש באינטרנט מפרופילים מרובים ונפרדים לחלוטין.</span><span class="sxs-lookup"><span data-stu-id="da619-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="da619-104">יכולות ההגנה הרחבות ביותר עבור נתוני Microsoft 365 הופכות לזמינים בעת הרשמה כמנוי ל- Enterprise Mobility + Security suite, הכוללת תכונות Microsoft Intune ו- Azure Active Directory Premium, כגון גישה מותנות.</span><span class="sxs-lookup"><span data-stu-id="da619-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="da619-105">לכל הפחות, תרצה לפרוס מדיניות גישה מותנית אשר (1) מאפשרת למשתמשים להתחבר ממכשירים ניידים ל- Microsoft Edge עבור iOS ו- Android, ו- (2) מיישם מדיניות הגנה מפני יישומים של Microsoft Intune המספקת חוויית גלישה מוגנת.</span><span class="sxs-lookup"><span data-stu-id="da619-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="da619-106">כדי להבין כיצד ניתן להשתמש בגישה ומדיניות מותנים, ראה:</span><span class="sxs-lookup"><span data-stu-id="da619-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="da619-107">החלת פריטי מדיניות גישה מותנים של Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="da619-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="da619-108">יצירת מדיניות הגנה על אפליקציית Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="da619-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="da619-109">שימוש בהתחברות יחידה עבור יישומי אינטרנט המחוברים ל- Azure Active Directory בדפדפנים המוגנים על-ידי מדיניות</span><span class="sxs-lookup"><span data-stu-id="da619-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="da619-110">שימוש בתצורת אפליקציה לניהול חוויית הגלישה</span><span class="sxs-lookup"><span data-stu-id="da619-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="da619-111">אפשר שימוש בחשבונות בעבודה ובלימודים בלבד</span><span class="sxs-lookup"><span data-stu-id="da619-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="da619-112">פריסת מדיניות תצורה כללית של יישום</span><span class="sxs-lookup"><span data-stu-id="da619-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="da619-113">פריסת מדיניות תצורת יישום עבור הגנה על נתונים</span><span class="sxs-lookup"><span data-stu-id="da619-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="da619-114">שימוש ב- Microsoft Endpoint Manager כדי לפרוס מדיניות תצורה של יישום</span><span class="sxs-lookup"><span data-stu-id="da619-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="da619-115">כדי ללמוד כיצד לגשת ליומני יישומים מנוהלים, ראה [שימוש ב- Microsoft Edge עבור iOS ו- Android כדי לגשת ליומני יישומים מנוהלים](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="da619-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
