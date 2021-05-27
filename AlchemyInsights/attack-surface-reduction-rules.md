---
title: כללי הפחתת פני השטח של תקיפה
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676232"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="b1d63-102">כללי הפחתת פני השטח של תקיפה</span><span class="sxs-lookup"><span data-stu-id="b1d63-102">Attack surface reduction rules</span></span>

<span data-ttu-id="b1d63-103">אי-הכללה של קבצים או תיקיות עשויה להפחית באופן חמור את ההגנה המסופקת על-ידי כללי הפחתת פני השטח של התקיפה.</span><span class="sxs-lookup"><span data-stu-id="b1d63-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="b1d63-104">ניתן להפעיל קבצים שנחסמו על-ידי כלל, ולא הדוח או אירוע.</span><span class="sxs-lookup"><span data-stu-id="b1d63-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="b1d63-105">אי-הכללה חלה על כל הכללים המאפשרים אי-הכללה.</span><span class="sxs-lookup"><span data-stu-id="b1d63-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="b1d63-106">אי-הכללות של ASR משתמשות באותו תחביר אנטי-וירוס של Microsoft Defender אי-הכללות.</span><span class="sxs-lookup"><span data-stu-id="b1d63-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="b1d63-107">לקבלת פרטים, ראה [קביעת תצורה ואימות של אי-הכללות עבור אנטי-וירוס של Microsoft Defender סריקות](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="b1d63-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="b1d63-108">כדי להימנע מבעיות, [עיין בטעויות נפוצות כדי להימנע בעת הגדרת אי-הכללות](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="b1d63-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="b1d63-109">לא כל כללי ASR תומכים בהכללות.</span><span class="sxs-lookup"><span data-stu-id="b1d63-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="b1d63-110">כדי לאמת אם הכלל שלך תומך בהיכללות, עיין בטבלה כללי [הפחתת פני השטח של התקפה](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="b1d63-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="b1d63-111">כללי הפחתת פני השטח של תקיפה</span><span class="sxs-lookup"><span data-stu-id="b1d63-111">Attack surface reduction rules</span></span>

<span data-ttu-id="b1d63-112">שטח התקיפה של הארגון שלך כולל את כל המקומות בהם תוקף עלול לסכן מכשירים או רשתות ארגוניים.</span><span class="sxs-lookup"><span data-stu-id="b1d63-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="b1d63-113">הפחתת פני השטח של התקיפה משמעה הגנה על המכשירים והרשת של הארגון, מה שמשאיר תוקפים עם פחות דרכים לביצוע תקיפות.</span><span class="sxs-lookup"><span data-stu-id="b1d63-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="b1d63-114">קביעת התצורה של כללי הפחתת פני השטח של התקפה ב- Microsoft Defender עבור נקודת קצה יכולה לעזור.</span><span class="sxs-lookup"><span data-stu-id="b1d63-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="b1d63-115">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="b1d63-115">For more information, see:</span></span>

- [<span data-ttu-id="b1d63-116">מפה GUID של כלל ASR לשם</span><span class="sxs-lookup"><span data-stu-id="b1d63-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="b1d63-117">דרישות כללי ASR:</span><span class="sxs-lookup"><span data-stu-id="b1d63-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="b1d63-118">Windows 10 Pro, גירסה 1709 ואילך</span><span class="sxs-lookup"><span data-stu-id="b1d63-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="b1d63-119">Windows 10 Enterprise, גירסה 1709 ואילך</span><span class="sxs-lookup"><span data-stu-id="b1d63-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="b1d63-120">Windows Server, גירסה 1803 (ערוץ חצי שנתי) ואילך</span><span class="sxs-lookup"><span data-stu-id="b1d63-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="b1d63-121">זהה את האי-הכללה הנכונה להחלה</span><span class="sxs-lookup"><span data-stu-id="b1d63-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="b1d63-122">חפש את eventID 1121 או 1122 ביומן Microsoft-Windows-Windows Defender/Operational.</span><span class="sxs-lookup"><span data-stu-id="b1d63-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="b1d63-123">להעריך את תרחיש הבלוק ואת ההקשר ואשר שיש לבטל חסימה של תרחיש זה.</span><span class="sxs-lookup"><span data-stu-id="b1d63-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="b1d63-124">קרא את הערך נתיב בפרטי האירוע, שהוא הערך המגדיר את האי-הכללה.</span><span class="sxs-lookup"><span data-stu-id="b1d63-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="b1d63-125">הפוך את האי-הכללה לקפדן ככל האפשר.</span><span class="sxs-lookup"><span data-stu-id="b1d63-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="b1d63-126">החל תו כללי כאשר יש צורך (לדוגמה, החלף משתנה משתמש).</span><span class="sxs-lookup"><span data-stu-id="b1d63-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="b1d63-127">החל את האי-הכללה בהתאם לצרכי הפריסה שלך.</span><span class="sxs-lookup"><span data-stu-id="b1d63-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="b1d63-128">לקבלת פרטים, ראה התאמה אישית [של כללי הפחתת פני השטח של התקפה](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="b1d63-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="b1d63-129">אי הכללה אינה מכובדת</span><span class="sxs-lookup"><span data-stu-id="b1d63-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="b1d63-130">קבע אם הכלל תומך בהיכללות.</span><span class="sxs-lookup"><span data-stu-id="b1d63-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="b1d63-131">לקבלת פרטים, ראה כללי [צמצום פני השטח של תקיפה](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="b1d63-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="b1d63-132">סקור את האי-הכללות שהוחלו ואמת עם נתוני האירוע עבור שגיאות הקלדה או תווים כלליים שלא פירטת כהלכה.</span><span class="sxs-lookup"><span data-stu-id="b1d63-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="b1d63-133">לקבלת מידע נוסף, ראה [סוגי אי-הכללה נתמכים](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="b1d63-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="b1d63-134">אם ההשפעה של הכלל היא גבוהה מדי, שקול להעביר את הכלל (בחזרה) למצב ביקורת כדי לבצע אימות נוסף.</span><span class="sxs-lookup"><span data-stu-id="b1d63-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="b1d63-135">לקבלת פרטים, ראה [בדיקת האופן שבו תכונות Microsoft Defender עבור נקודות קצה פועלות במצב ביקורת](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="b1d63-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="b1d63-136">אסוף נתוני תמיכה כדי לפתוח מקרה תמיכה באמצעות פקודה זו:</span><span class="sxs-lookup"><span data-stu-id="b1d63-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="b1d63-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="b1d63-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="b1d63-138">לקבלת מידע נוסף, ראה [בעיות עם מחשבים ל- Microsoft Defender עבור נקודות קצה.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="b1d63-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
