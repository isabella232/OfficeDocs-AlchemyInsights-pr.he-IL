---
title: פתרון בעיה ב-PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573726"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="5e676-102">פתרון בעיה ב-PRT</span><span class="sxs-lookup"><span data-stu-id="5e676-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="5e676-103">כדי שמכשיר כלשהו ישלים את האימות, עליו להיות רשום במלואו ובמצב טוב ולרכוש אסימון רענון ראשי (PRT).</span><span class="sxs-lookup"><span data-stu-id="5e676-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="5e676-104">תהליך ההרשמה להצטרפות היברידית תכלת מחייב מכשירים להיות ברשת של החברה.</span><span class="sxs-lookup"><span data-stu-id="5e676-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="5e676-105">היא פועלת גם באמצעות VPN, אך יש כמה אזהרות לכך.</span><span class="sxs-lookup"><span data-stu-id="5e676-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="5e676-106">שמענו שהלקוחות זקוקים לסיוע בפתרון בעיות בתהליך ההרשמה להצטרפות היברידית תכלת לספירה תחת נסיבות עבודה מרחוק.</span><span class="sxs-lookup"><span data-stu-id="5e676-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="5e676-107">להלן פירוט של המתרחש ' מתחת למכסה המנוע ' במהלך תהליך ההרשמה.</span><span class="sxs-lookup"><span data-stu-id="5e676-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="5e676-108">**סביבת אימות ענן (שימוש בסינכרון hash של הסיסמה תכלת או אימות מעבר)**</span><span class="sxs-lookup"><span data-stu-id="5e676-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="5e676-109">זרימת רישום זו נקראת גם "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="5e676-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="5e676-110">Windows 10 מגלה רשומת SCP בעת הכניסה של המשתמש למכשיר.</span><span class="sxs-lookup"><span data-stu-id="5e676-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="5e676-111">המכשיר מנסה תחילה לאחזר את פרטי הדייר מSCP בצד הלקוח ברישום [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="5e676-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="5e676-112">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)זה.</span><span class="sxs-lookup"><span data-stu-id="5e676-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="5e676-113">אם היא נכשלת, ההתקן מקיים תקשורת עם Active Directory מקומי (AD) כדי לקבל פרטי דייר מנקודת חיבור השירות (SCP).</span><span class="sxs-lookup"><span data-stu-id="5e676-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="5e676-114">כדי לאמת את SCP, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)זה.</span><span class="sxs-lookup"><span data-stu-id="5e676-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="5e676-115">אנו ממליצים לאפשר ל-SCP במודע ולהשתמש רק בSCP בצד הלקוח לצורך אימות ראשוני.</span><span class="sxs-lookup"><span data-stu-id="5e676-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="5e676-116">Windows 10 מנסה לקיים תקשורת עם התכלת AD תחת הקשר המערכת כדי לאמת את עצמו כנגד תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="5e676-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="5e676-117">באפשרותך לאמת אם המכשיר יכול לגשת למשאבי Microsoft תחת חשבון המערכת באמצעות קובץ ה-script של החיבור לרישום מכשירים.</span><span class="sxs-lookup"><span data-stu-id="5e676-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="5e676-118">Windows 10 יוצר אישור בחתימה עצמית ומאחסן אותו תחת אובייקט המחשב בהודעה מקומית.</span><span class="sxs-lookup"><span data-stu-id="5e676-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="5e676-119">פעולה זו דורשת שורת המראה לבקר תחום.</span><span class="sxs-lookup"><span data-stu-id="5e676-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="5e676-120">אובייקט מכשיר המכיל אישור מסונכרן לכיוון התכלת לספירה דרך תכלת AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5e676-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="5e676-121">מחזור הסינכרון מתבצע כל 30 דקות כברירת מחדל, אך הדבר תלוי בקביעת התצורה של התחברות של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="5e676-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="5e676-122">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)זה.</span><span class="sxs-lookup"><span data-stu-id="5e676-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="5e676-123">בשלב זה, תוכל לראות את התקן הנושא במצב "ממתין" תחת מכשיר להב של הפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="5e676-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="5e676-124">בכניסה למשתמש הבא ל-Windows 10, הרישום יושלם.</span><span class="sxs-lookup"><span data-stu-id="5e676-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="5e676-125">אם אתה משתמש ב-VPN ותהליך התחברות מתנתק מסיים את קישוריות התחום, באפשרותך להפעיל את הרישום באופן ידני:</span><span class="sxs-lookup"><span data-stu-id="5e676-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="5e676-126">הנפק dsregcmd/join באופן מקומי בבקשה לניהול או באמצעות מרחוק דרך PSExec למחשב.</span><span class="sxs-lookup"><span data-stu-id="5e676-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="5e676-127">לדוגמה, PsExec-s \\ win10client01 cmd, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="5e676-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="5e676-128">לקבלת פרטים נוספים על בעיות הצטרפות היברידיות, ראה [פתרון בעיות במכשירים](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="5e676-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
