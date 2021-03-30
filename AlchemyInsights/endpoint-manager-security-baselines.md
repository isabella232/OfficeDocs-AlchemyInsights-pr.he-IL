---
title: EndPoint Manager - תוכניות בסיסיות של אבטחה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420880"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="9aa6f-102">EndPoint Manager - תוכניות בסיסיות של אבטחה</span><span class="sxs-lookup"><span data-stu-id="9aa6f-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="9aa6f-103">תוכניות בסיסיות אבטחה הן קבוצות מוגדרות מראש של הגדרות Windows, שיעזור לך להחיל את הגדרות האבטחה המומלצות על-ידי צוותי האבטחה הרלוונטיים.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="9aa6f-104">ניתן להתאים אישית תוכניות בסיסיות אלה כדי לספק רק את ההגדרות והערכים הרצויים.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="9aa6f-105">לקבלת מידע נוסף אודות תוכניות בסיסיות של אבטחה, ראה [שימוש בתוכנית בסיסית של אבטחה כדי לקבוע את התצורה של מכשירי Windows 10 ב- Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="9aa6f-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="9aa6f-106">כיום זמינים תוכניות בסיסיות עבור מוצרים אלה:</span><span class="sxs-lookup"><span data-stu-id="9aa6f-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="9aa6f-107">הגדרות אבטחה של Windows MDM</span><span class="sxs-lookup"><span data-stu-id="9aa6f-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="9aa6f-108">Microsoft Defender עבור אבטחת EndPoint</span><span class="sxs-lookup"><span data-stu-id="9aa6f-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="9aa6f-109">מייקרוסופט אדג'</span><span class="sxs-lookup"><span data-stu-id="9aa6f-109">Microsoft Edge</span></span>

<span data-ttu-id="9aa6f-110">כל אחת מ בסיסית מתעדכנת מעת לעת ומופץ בגירסאות מצטברות.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="9aa6f-111">כל גירסה מוסיפה או מסירה הגדרות מהגירסה הקודמת כדי להבטיח שה בסיסית תיפגש עם ההנחיות הנוכחיות.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="9aa6f-112">מסוף תוכניות בסיסיות של אבטחה באבטחת נקודות קצה מאפשר השוואה בין גירסאות שונות על-ידי הפיכת השינויים מגירסה לגירסה לגלויים.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="9aa6f-113">לקבלת הדרכה כיצד לשנות בצורה היעילה ביותר את גירסת התוכנית הבסיסית שנפרסת, ראה [ניהול פרופילי תוכנית בסיסית של אבטחה ב- Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="9aa6f-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="9aa6f-114">לאחר פריסת תוכנית בסיסית של אבטחה, באפשרותך לנטר את מצב הפריסה וביקורות ההגדרות על בסיס מכשיר אחר מכשיר.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="9aa6f-115">**הערה:** נתוני הדיווח עבור תוכניות בסיסיות עשויים להתקדם עד 24 שעות מהפריסה הראשונית למכשיר ועד 6 שעות לעדכונים נוספים.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="9aa6f-116">הסיבה הנפוצה ביותר להגדרה בסיסית אינה חלה היא משום שהגדרה זו נמצאת בשימוש בפרופיל אחר.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="9aa6f-117">ניתן לחקור תרחיש זה עבור מכשיר ספציפי על-ידי בחירת מכשיר זה מתוך הצומת מצב התקן של פרופיל 'תוכנית בסיסית של אבטחה'.</span><span class="sxs-lookup"><span data-stu-id="9aa6f-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="9aa6f-118">לקבלת פרטים, ראה [פתרון התנגשויות עבור תוכניות בסיסיות של אבטחה.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="9aa6f-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>