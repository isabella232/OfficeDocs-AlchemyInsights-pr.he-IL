---
title: תכניות בסיסיות של EndPoint Manager - Security
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440885"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="68ab3-102">תכניות בסיסיות של EndPoint Manager - Security</span><span class="sxs-lookup"><span data-stu-id="68ab3-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="68ab3-103">תוכניות אבטחה בסיסיות הן קבוצות של הגדרות Windows מוגדרות מראש שעוזרות לך להחיל את הגדרות האבטחה שצוותי אבטחה רלוונטיים ממליצים להם.</span><span class="sxs-lookup"><span data-stu-id="68ab3-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="68ab3-104">התוכניות הבסיסיות הללו פתוחות להתאמות שמאפשרות למסור רק את ההגדרות והערכים הרצויים.</span><span class="sxs-lookup"><span data-stu-id="68ab3-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="68ab3-105">למידע נוסף על תוכניות אבטחה בסיסיות ראה [שימוש בתוכניות אבטחה בסיסיות לקביעת תצורה של מכשירי Windows 10 ב- Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="68ab3-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="68ab3-106">נכון לעכשיו, יש תוכניות בסיסיות למוצרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="68ab3-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="68ab3-107">הגדרות אבטחה של Windows MDM</span><span class="sxs-lookup"><span data-stu-id="68ab3-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="68ab3-108">Microsoft Defender ל- EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="68ab3-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="68ab3-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="68ab3-109">Microsoft Edge</span></span>

<span data-ttu-id="68ab3-110">כל אחת מהתוכניות הבסיסיות מתעדכנת מעת לעת ומופצת בגרסאות מצטברות.</span><span class="sxs-lookup"><span data-stu-id="68ab3-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="68ab3-111">בכל גרסה מתווספות או נגרעות הגדרות מהגרסה הקודמת כדי להבטיח שהתוכנית הבסיסית עומדת בדרישות הקו המנחה העדכני.</span><span class="sxs-lookup"><span data-stu-id="68ab3-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="68ab3-112">מסוף תכניות האבטחה הבסיסיות ב- Endpoint Security מאפשר השוואה בין גרסאות שונות בכך שהוא מאפשר לראות את ההבדלים בין גרסה אחת לשנייה.</span><span class="sxs-lookup"><span data-stu-id="68ab3-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="68ab3-113">ראו הדרכה על השינויים היעילים ביותר לכל גרסה של תכנית בסיסית כאן [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="68ab3-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="68ab3-114">לאחר התקנת תוכנית אבטחה בסיסית באפשרותך לנטר את מצב ההתקנה ולבחון מחדש הגדרות של מכשיר אחר מכשיר.</span><span class="sxs-lookup"><span data-stu-id="68ab3-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="68ab3-115">**שים לב:** ייתכן שיחלפו עד 24 שעות עד הופעתם של נתוני דיווח על תוכניות בסיסיות מהתקנה הראשונית במכשיר. בעדכונים נוספים, עד שש שעות.</span><span class="sxs-lookup"><span data-stu-id="68ab3-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="68ab3-116">הסיבה הנפוצה ביותר לאי החלה של הגדרת תוכנית בסיסית היא שאותה הגדרה נמצאת בשימוש בפרופיל אחר.</span><span class="sxs-lookup"><span data-stu-id="68ab3-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="68ab3-117">אפשר לבדוק את התרחיש בכל מכשיר על-ידי בחירתו בצומת 'מצב מכשיר' בפרופיל ה- Security Baseline.</span><span class="sxs-lookup"><span data-stu-id="68ab3-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="68ab3-118">ראה מידע מפורט כאן [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="68ab3-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>