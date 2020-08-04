---
title: בעיות הקשורות ל-VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555237"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="5042c-102">בעיות הקשורות ל-VPN</span><span class="sxs-lookup"><span data-stu-id="5042c-102">VPN related issues</span></span>

<span data-ttu-id="5042c-103">יישום מוצלח של קישוריות VPN עבור לקוחות MDM תלוי בפרופיל שנפרס המשקף בצורה נכונה את הדרישות של תשתית ה-VPN.</span><span class="sxs-lookup"><span data-stu-id="5042c-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="5042c-104">לקבלת ההגדרות המתאימות עבור פלטפורמות הלקוח שאתה חוקר, ראה:</span><span class="sxs-lookup"><span data-stu-id="5042c-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="5042c-105">Windows 10 והגדרות התקן הולוגרפית של Windows כדי להוסיף חיבורי VPN באמצעות Intune</span><span class="sxs-lookup"><span data-stu-id="5042c-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="5042c-106">הוסף הגדרות VPN על iOS ו-iPadOS התקנים ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5042c-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="5042c-107">הגדרות אנדרואיד התקן להגדיר VPN ב Intune</span><span class="sxs-lookup"><span data-stu-id="5042c-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="5042c-108">הוסף הגדרות VPN על התקני macOS ב-Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5042c-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="5042c-109">אם פרופיל ה-VPN משתמש באימות המבוסס על אישורים, ודא שאישור הבסיס ופרופילי אישורי אימות הלקוח המקושרים לפרופיל ה-VPN נפרסים בהצלחה.</span><span class="sxs-lookup"><span data-stu-id="5042c-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="5042c-110">**סוגיות נפוצות**</span><span class="sxs-lookup"><span data-stu-id="5042c-110">**Common Issues**</span></span>

<span data-ttu-id="5042c-111">**הפרסתי פרופיל VPN למכשיר. Intune מראה כי זה היה מוצלח, אבל המכשיר אינו מתחבר ל-VPN.**</span><span class="sxs-lookup"><span data-stu-id="5042c-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="5042c-112">מצב מוצלח פירושו שIntune בהצלחה את הפרופיל כפי שהוגדר.</span><span class="sxs-lookup"><span data-stu-id="5042c-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="5042c-113">עם זאת, ייתכן שתצורות אלה לא יתאימו לדרישות הרשת ו/או האימות שלך.</span><span class="sxs-lookup"><span data-stu-id="5042c-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="5042c-114">סקירת יומני רישום בשירות התשתית והאימות (בשרת VPN ובשרת NPS/Radius) לקבלת פרטים נוספים אודות ניסיון החיבור.</span><span class="sxs-lookup"><span data-stu-id="5042c-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="5042c-115">ייתכן שתצטרך לעבוד עם צוות תשתית הרשת, או ספק ה-VPN של ספק חיצוני, כדי לאסוף ולסקור יומני רישום.</span><span class="sxs-lookup"><span data-stu-id="5042c-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="5042c-116">**כאשר אני מגדיר VPN מותאם אישית עבור iOS, התכונה per-app VPN לא נעשה זמין.**</span><span class="sxs-lookup"><span data-stu-id="5042c-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="5042c-117">Per-app VPN עבור מכשירי iOS ב Intune זמין כעת רשימה מסוימת של ספקים ושותפים, מי חייב גם לעמוד בדרישות המוקדמות אישור לפני הגדרת VPN לפי app.</span><span class="sxs-lookup"><span data-stu-id="5042c-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="5042c-118">לקבלת מידע נוסף, ראה [הגדרת לכל יישום רשת פרטית וירטואלית (VPN) עבור iOS/iPadOS התקנים ב Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="5042c-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="5042c-119">לקבלת מידע נוסף על כל סוגי החיבור VPN ב Intune, ראה [יצירת פרופילי vpn כדי להתחבר שרתי vpn ב Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="5042c-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="5042c-120">**iOS On-דרישה VPN אינו מפעיל כאשר הגישה לתחום שתצורתו נקבעה**</span><span class="sxs-lookup"><span data-stu-id="5042c-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="5042c-121">כדי לבדוק את הגדרות ה-VPN האוטומטיות, הגדר את הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5042c-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="5042c-122">ברצוני לבצע את הפעולות הבאות: **הערכת כל ניסיון לחיבור**</span><span class="sxs-lookup"><span data-stu-id="5042c-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="5042c-123">בחר אם להתחבר: **התחבר במידת הצורך**</span><span class="sxs-lookup"><span data-stu-id="5042c-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="5042c-124">כאשר משתמשים ניגשים לתחומים אלה: *שם תחום* **יעד**</span><span class="sxs-lookup"><span data-stu-id="5042c-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="5042c-125">אם התצורה שלעיל אינה מוצלחת, הוסף את הרכיב הבא:</span><span class="sxs-lookup"><span data-stu-id="5042c-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="5042c-126">כאשר כתובת URL זו אינה נגישה, הכוח לחבר את ה-VPN: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="5042c-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>