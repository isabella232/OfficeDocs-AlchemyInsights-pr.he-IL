---
title: אני נחסם על-ידי גישה מותנית עם התקן תואם
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035994"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="e2670-102">אני נחסם על-ידי גישה מותנית עם התקן תואם</span><span class="sxs-lookup"><span data-stu-id="e2670-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="e2670-103">**כלים מומלצים במיוחד**</span><span class="sxs-lookup"><span data-stu-id="e2670-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="e2670-104">[כלי פותר בעיות רישום המכשירים](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -כלי מקיף שעוזר לפתור בעיות ברישום המכשירים הנפוצים ביותר.</span><span class="sxs-lookup"><span data-stu-id="e2670-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="e2670-105">[בדיקת קובץ script של קישוריות לרישום מכשירים](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -כלי המשמש כדי להבטיח שההתקן יוכל לגשת לנקודות קצה של רישום מכשירים תחת חשבון המערכת.</span><span class="sxs-lookup"><span data-stu-id="e2670-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="e2670-106">[קובץ Script לניקוי התקן תכלת](https://github.com/mzmaili/AzureADDeviceCleanup) -כלי המשמש לחיפוש ולניהול של מכשירים ישנים בסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="e2670-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="e2670-107">להלן כמה סיבות נפוצות לכך שגישה מותנית עשויה להיכשל עבור מכשיר תואם או מדוע ייתכן **שהמשתמשים** שלך מקבלים את ההודעה במהלך בקשת כניסה למשאב ארגוני.</span><span class="sxs-lookup"><span data-stu-id="e2670-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="e2670-108">**המכשיר אינו נמצא במצב התקן נדרש עם MDM**:</span><span class="sxs-lookup"><span data-stu-id="e2670-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="e2670-109">ודא שההתקן נרשם עם ספק MDM מאושר, כגון ' שלחן ' *ומסומן כתואם*.</span><span class="sxs-lookup"><span data-stu-id="e2670-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="e2670-110">לקבלת מידע נוסף אודות המנגינה, ראה [מסמך](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)זה.</span><span class="sxs-lookup"><span data-stu-id="e2670-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="e2670-111">לקבלת הבנה טובה יותר של תאימות מכשירים וכוונון, ראה [שימוש במדיניות תאימות כדי להגדיר כללים עבור מכשירים שאתה מנהל באמצעות ' כוונון](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)'.</span><span class="sxs-lookup"><span data-stu-id="e2670-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="e2670-112">אם אתה נתקל בבעיות ברישום מכשיר באמצעות ' כוונון ', מצא את פרטי פתרון הבעיות [בפתרון בעיות בהרשמת מכשירים ב-Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e2670-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="e2670-113">לקבלת תמיכה נוספת, צור בקשה לתמיכה.</span><span class="sxs-lookup"><span data-stu-id="e2670-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="e2670-114">כדי לעשות זאת, בקר [בדף העזרה והתמיכה של כוונון](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span><span class="sxs-lookup"><span data-stu-id="e2670-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="e2670-115">**המכשיר אינו מצורף לרשת הארגונים**:</span><span class="sxs-lookup"><span data-stu-id="e2670-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="e2670-116">כדי לגשת למשאבים ארגוניים, המכשיר צריך להיות מחובר לרשת של הארגון, באמצעות חיבור ישיר או רשת וירטואלית פרטית (VPN), וכן הצטרפות למדריך הכתובות המקומי או התכלת של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e2670-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="e2670-117">כדי להצטרף להתקן עבודה לרשת הארגונית, ראה [הצטרפות למכשיר העבודה שלך לרשת של הארגון שלך](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span><span class="sxs-lookup"><span data-stu-id="e2670-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="e2670-118">כדי לרשום התקן אישי/BYOD, ראה [רישום המכשיר האישי שלך ברשת של הארגון](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)שלך.</span><span class="sxs-lookup"><span data-stu-id="e2670-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="e2670-119">כדי לאמת אם המכשיר הצטרף לרשת, באפשרותך לבצע את השלבים עבור התקנים רשומים [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) או מכשירי עבודה [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span><span class="sxs-lookup"><span data-stu-id="e2670-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="e2670-120">כדי להרחיב את הבעיה לקישוריות רשת ארגונית, בצע את ההנחיות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e2670-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="e2670-121">היכנס ל-Windows באמצעות החשבון שלך בעבודה או בבית הספר, לדוגמה, alain@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="e2670-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="e2670-122">התחבר לרשת של הארגון שלך דרך VPN או DirectAccess.</span><span class="sxs-lookup"><span data-stu-id="e2670-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="e2670-123">לאחר שאתה מחובר, הקש על **מקש סמל Windows + L** כדי לנעול את המכשיר.</span><span class="sxs-lookup"><span data-stu-id="e2670-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="e2670-124">בטל את נעילת המכשיר באמצעות החשבון שלך בעבודה או בבית הספר ולאחר מכן נסה שוב לגשת ליישום או לשירות הבעייתי.</span><span class="sxs-lookup"><span data-stu-id="e2670-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="e2670-125">אם אתה רואה את ההודעה **לא ניתן להגיע שוב מהודעת השגיאה הבאה** , הבעיה עשויה להיות במקום אחר.</span><span class="sxs-lookup"><span data-stu-id="e2670-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="e2670-126">**מערכת ההפעלה אינה נתמכת**:</span><span class="sxs-lookup"><span data-stu-id="e2670-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="e2670-127">ודא שאתה מפעיל גירסה נתמכת של מערכת ההפעלה, כולל:</span><span class="sxs-lookup"><span data-stu-id="e2670-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="e2670-128">**לקוח windows**: windows 7 ואילך</span><span class="sxs-lookup"><span data-stu-id="e2670-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="e2670-129">**Windows server**: windows Server 2008 R2 ואילך</span><span class="sxs-lookup"><span data-stu-id="e2670-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="e2670-130">**macOS**: macos X ואילך</span><span class="sxs-lookup"><span data-stu-id="e2670-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="e2670-131">**Android ו-ios**: הגירסה העדכנית ביותר של android ו-ios מערכות הפעלה ניידות</span><span class="sxs-lookup"><span data-stu-id="e2670-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="e2670-132">**דפדפן אינטרנט אינו נתמך**:</span><span class="sxs-lookup"><span data-stu-id="e2670-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="e2670-133">חפש בדפדפנים נתמכים להלן.</span><span class="sxs-lookup"><span data-stu-id="e2670-133">Please find supported browsers below.</span></span> <span data-ttu-id="e2670-134">עבור תמיכה ב-Chrome עם Windows 1703 וגירסאות מתקדמות יותר, נדרשת סיומת של Windows 10 חשבונות.</span><span class="sxs-lookup"><span data-stu-id="e2670-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="e2670-135">עבור Edge 85 +, המשתמש צריך להיות מחובר כדי להעביר כהלכה את מידע תאימות המכשירים.</span><span class="sxs-lookup"><span data-stu-id="e2670-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="e2670-136">לקבלת פרטים נוספים, ראה [כאן](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="e2670-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="e2670-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="e2670-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="e2670-138">**Windows 8/8.1**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="e2670-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="e2670-139">**Windows 7**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="e2670-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="e2670-140">**iOS**: Microsoft Edge, כוונון דפדפן מנוהל, Safari</span><span class="sxs-lookup"><span data-stu-id="e2670-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="e2670-141">**Android**: **Microsoft Edge**: כוונון דפדפן מנוהל, כרום</span><span class="sxs-lookup"><span data-stu-id="e2670-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="e2670-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="e2670-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="e2670-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="e2670-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="e2670-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="e2670-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="e2670-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="e2670-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="e2670-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="e2670-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="e2670-147">**macOS**: Chrome, Safari</span><span class="sxs-lookup"><span data-stu-id="e2670-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="e2670-148">חפש מידע נוסף בנושא **אין באפשרותך לקבל** את ההודעה ולפתור את השלבים [כאן](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span><span class="sxs-lookup"><span data-stu-id="e2670-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
