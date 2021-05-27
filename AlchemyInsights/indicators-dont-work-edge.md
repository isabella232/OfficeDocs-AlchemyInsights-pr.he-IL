---
title: מחוונים לא פועלים באמצעות דפדפן Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676242"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="339e7-102">מחוונים לא פועלים באמצעות דפדפן Edge</span><span class="sxs-lookup"><span data-stu-id="339e7-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="339e7-103">לאחר יצירת מחוון, הוא אינו מכובד על-ידי Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="339e7-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="339e7-104">לקבלת מידע נוסף, ראה [יצירת מחוונים עבור כתובות URL וכתובות URL/תחומים.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="339e7-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="339e7-105">שלב 1: ודא שהפעולות הבאות</span><span class="sxs-lookup"><span data-stu-id="339e7-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="339e7-106">ודא כי המחוון נכון (אין שגיאות הקלדה ב- IP/URL, הפעולה הנכונה, קבוצות ה- RBAC הנכונות).</span><span class="sxs-lookup"><span data-stu-id="339e7-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="339e7-107">המתן שעתיים לפחות לאחר יצירת המחוון כדי לקחת בחשבון כל השהיה אפשרית.</span><span class="sxs-lookup"><span data-stu-id="339e7-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="339e7-108">ודא שהמערכת(ים) המשולבות ב- Microsoft Defender עבור נקודת קצה.</span><span class="sxs-lookup"><span data-stu-id="339e7-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="339e7-109">ודא שמערכת(ים) זו יכולה לקיים תקשורת עם הענן.</span><span class="sxs-lookup"><span data-stu-id="339e7-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="339e7-110">ודא ש- Smartscreen זמין וניתן להגיע אליו על-ידי [מחשב שלך](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="339e7-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="339e7-111">שלב 2: פתרון הבעיה הפוטנציאלית</span><span class="sxs-lookup"><span data-stu-id="339e7-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="339e7-112">ודא שהלקוח לעמוד בדרישות.</span><span class="sxs-lookup"><span data-stu-id="339e7-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="339e7-113">לקבלת פרטים, ראה [יצירת מחוונים עבור כתובות URL וכתובות URL/תחומים](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="339e7-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="339e7-114">ודא שאתה משתמש בגירסה העדכנית ביותר של דפדפן Edge.</span><span class="sxs-lookup"><span data-stu-id="339e7-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="339e7-115">כדי לגלות את הגירסה העדכנית ביותר, [ראה גלה איזו גירסה Microsoft Edge שלך.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="339e7-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="339e7-116">הפעל מחדש את דפדפן Edge.</span><span class="sxs-lookup"><span data-stu-id="339e7-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="339e7-117">נווט אל האתר שעבורו הגדרת מחוון.</span><span class="sxs-lookup"><span data-stu-id="339e7-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="339e7-118">אם האתר אינו מופיע כצפוי, המשך לשלב 3.</span><span class="sxs-lookup"><span data-stu-id="339e7-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="339e7-119">שלב 3: איסוף נתונים</span><span class="sxs-lookup"><span data-stu-id="339e7-119">Step 3: Collect data</span></span>

- <span data-ttu-id="339e7-120">איסוף **נתוני אבחון של MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="339e7-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="339e7-121">לקבלת הוראות, ראה [בעיות עם מחשבים ל- Microsoft Defender עבור נקודת קצה.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="339e7-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="339e7-122">אם אתה מרגיש בנוח להתקין ולאסוף מעקב אחר Fiddler, ראה [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="339e7-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="339e7-123">אם אתה מעדיף הדרכה מהתמיכה של Microsoft, בחר את סמל התמיכה להלן כדי לפתוח מקרה תמיכה.</span><span class="sxs-lookup"><span data-stu-id="339e7-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
