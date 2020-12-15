---
title: שימוש ב-Microsoft intune לניהול גישה לאינטרנט ב-Microsoft Edge עבור iOS ו-Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678257"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="57546-102">שימוש ב-Microsoft intune לניהול גישה לאינטרנט ב-Microsoft Edge עבור iOS ו-Android</span><span class="sxs-lookup"><span data-stu-id="57546-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="57546-103">Microsoft Edge עבור iOS ו-Android מאפשר למשתמש לגלוש באינטרנט מתוך פרופילים נפרדים מרובים ונפרדים לחלוטין.</span><span class="sxs-lookup"><span data-stu-id="57546-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="57546-104">יכולות ההגנה הרחבות ביותר עבור נתוני Microsoft 365 הופכות לזמינות כאשר אתה נרשם כמנוי לניידות Enterprise + חבילת אבטחה, הכוללת את Microsoft intune ו-תכלת Active Directory תכונות פרמיום, כגון גישה מותנית.</span><span class="sxs-lookup"><span data-stu-id="57546-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="57546-105">לכל הפחות, תרצה לפרוס מדיניות גישה מותנית ש-(1) מאפשרת למשתמשים להתחבר ממכשירים ניידים ל-Microsoft Edge עבור iOS ו-Android ו-(2) מיישמת מדיניות הגנה של Microsoft intune-הגנת יישומים המספקת חוויית גלישה מוגנת.</span><span class="sxs-lookup"><span data-stu-id="57546-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="57546-106">כדי להבין כיצד באפשרותך להשתמש בגישה מותנית ובמדיניות, ראה:</span><span class="sxs-lookup"><span data-stu-id="57546-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="57546-107">החלת מדיניות גישה מותנית של תכלת Active Directory</span><span class="sxs-lookup"><span data-stu-id="57546-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="57546-108">יצירת מדיניות הגנת יישומים של Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="57546-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="57546-109">שימוש בכניסה יחידה עבור התכלת Active Directory – יישומי אינטרנט מחוברים בדפדפנים המוגנים באמצעות מדיניות</span><span class="sxs-lookup"><span data-stu-id="57546-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="57546-110">שימוש בקביעת תצורה של יישומים כדי לנהל את חוויית הגלישה</span><span class="sxs-lookup"><span data-stu-id="57546-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="57546-111">מתן אפשרות לשימוש בחשבונות עבודה ובבית ספר בלבד</span><span class="sxs-lookup"><span data-stu-id="57546-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="57546-112">פריסת מדיניות של תצורת יישומים כלליים</span><span class="sxs-lookup"><span data-stu-id="57546-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="57546-113">פריסת מדיניות תצורת יישומים עבור הגנה על נתונים</span><span class="sxs-lookup"><span data-stu-id="57546-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="57546-114">השתמש במנהל נקודות הקצה של Microsoft כדי לפרוס מדיניות תצורת יישומים</span><span class="sxs-lookup"><span data-stu-id="57546-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="57546-115">כדי ללמוד כיצד לגשת ליומני היישומים המנוהלים, ראה [שימוש ב-Microsoft Edge עבור iOS וב-Android כדי לגשת ליומני יישומים מנוהלים](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="57546-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
