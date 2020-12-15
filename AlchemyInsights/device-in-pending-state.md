---
title: התקן במצב ממתין
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678481"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="ad61d-102">התקן במצב ממתין</span><span class="sxs-lookup"><span data-stu-id="ad61d-102">Device in pending state</span></span>

<span data-ttu-id="ad61d-103">**דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="ad61d-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="ad61d-104">אם אתה מגדיר רישומי מכשירים בפעם הראשונה, ודא שהצגת [מבוא לניהול מכשירים ב-תכלת Active Directory (תכלת לספירה)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) שידריך אותך לגבי אופן השגת מכשירים תחת השליטה של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="ad61d-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="ad61d-105">אם אתה מבצע רישום של מכשירים בתוך התכלת לספירה ישירות ומצרף אותם לתוך המנגינה, עליך לוודא שהגדרת את האפשרות ' שאתה מגדיר ' את האפשרות ' שאתה [מגדיר](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) את האפשרות ' והרישוי הקודם מתבצע. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ad61d-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="ad61d-106">ודא שאתה מורשה לבצע פעולות ב-תכלת AD ובמודעה מקומית.</span><span class="sxs-lookup"><span data-stu-id="ad61d-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="ad61d-107">רק מנהל מערכת כללי בתכלת לספירה יכול לנהל הגדרות עבור רישומי מכשירים.</span><span class="sxs-lookup"><span data-stu-id="ad61d-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="ad61d-108">בנוסף, אם אתה מגדיר רישומים אוטומטיים ב-Active Directory המקומי שלך, יהיה עליך להיות מנהל מערכת של Active Directory ו-AD FS (אם ישים).</span><span class="sxs-lookup"><span data-stu-id="ad61d-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="ad61d-109">תהליך ההרשמה להצטרפות היברידית תכלת מחייב מכשירים להיות ברשת הארגונית.</span><span class="sxs-lookup"><span data-stu-id="ad61d-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="ad61d-110">היא פועלת גם באמצעות VPN, אך יש כמה אזהרות לכך.</span><span class="sxs-lookup"><span data-stu-id="ad61d-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="ad61d-111">שמענו את הלקוחות זקוקים לסיוע בפתרון בעיות בתהליך ההרשמה להצטרפות היברידית תכלת לספירה תחת נסיבות עבודה מרוחקות.</span><span class="sxs-lookup"><span data-stu-id="ad61d-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="ad61d-112">**סביבת אימות ענן (שימוש בסינכרון hash של הסיסמה תכלת או אימות מעבר)**</span><span class="sxs-lookup"><span data-stu-id="ad61d-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="ad61d-113">זרימת רישום זו נקראת גם "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="ad61d-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="ad61d-114">להלן פירוט של מה שקורה במהלך תהליך ההרשמה:</span><span class="sxs-lookup"><span data-stu-id="ad61d-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="ad61d-115">Windows 10 מגלה את רשומת נקודת חיבור השירות (SCP) כאשר המשתמש נכנס למכשיר.</span><span class="sxs-lookup"><span data-stu-id="ad61d-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="ad61d-116">המכשיר מנסה תחילה לאחזר את פרטי הדייר מSCP בצד הלקוח ברישום [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="ad61d-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="ad61d-117">לקבלת מידע נוסף, ראה [מסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="ad61d-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="ad61d-118">אם היא נכשלת, ההתקן מקיים תקשורת עם Active Directory מקומי כדי לקבל מידע אודות הדייר מ-SCP.</span><span class="sxs-lookup"><span data-stu-id="ad61d-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="ad61d-119">כדי לאמת את SCP, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)זה.</span><span class="sxs-lookup"><span data-stu-id="ad61d-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="ad61d-120">אנו ממליצים להפוך את SCP לזמין ב-Active Directory ורק באמצעות SCP בצד הלקוח לצורך אימות ראשוני.</span><span class="sxs-lookup"><span data-stu-id="ad61d-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="ad61d-121">Windows 10 מנסה לקיים תקשורת עם התכלת AD תחת הקשר המערכת כדי לאמת את עצמו כנגד תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="ad61d-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="ad61d-122">באפשרותך לאמת אם המכשיר יכול לגשת למשאבי Microsoft תחת חשבון המערכת באמצעות [קובץ ה-script של החיבור לרישום מכשירים](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="ad61d-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="ad61d-123">Windows 10 יוצר אישור בחתימה עצמית ומאחסן אותו תחת אובייקט המחשב ב-Active Directory מקומי.</span><span class="sxs-lookup"><span data-stu-id="ad61d-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="ad61d-124">פעולה זו דורשת שורת המראה לבקר תחום.</span><span class="sxs-lookup"><span data-stu-id="ad61d-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="ad61d-125">אובייקט מכשיר המכיל אישור מסתנכרן עם התכלת לספירה באמצעות התחברות לספירה.</span><span class="sxs-lookup"><span data-stu-id="ad61d-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="ad61d-126">מחזור הסינכרון מתבצע כל 30 דקות כברירת מחדל, אך תלוי בקביעת התצורה של התחברות של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="ad61d-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="ad61d-127">לקבלת מידע נוסף, עיין [במסמך](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)זה.</span><span class="sxs-lookup"><span data-stu-id="ad61d-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="ad61d-128">בשלב זה, תוכל לראות את התקן הנושא במצב "**ממתין**" תחת מכשיר להב של הפורטל התכלת.</span><span class="sxs-lookup"><span data-stu-id="ad61d-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="ad61d-129">בכניסה למשתמש הבא ל-Windows 10, הרישום יושלם.</span><span class="sxs-lookup"><span data-stu-id="ad61d-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ad61d-130">אם אתה מתחבר ל-VPN והתנתקות/הכניסה מסתיימת את קישוריות התחום, באפשרותך להפעיל את הרישום באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="ad61d-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="ad61d-131">כדי לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="ad61d-131">To do that:</span></span>
    >
    > <span data-ttu-id="ad61d-132">הנפק `dsregcmd /join` בקשה מקומית בבקשה למנהלי מערכת או באמצעות מרחוק דרך PSExec למחשב.</span><span class="sxs-lookup"><span data-stu-id="ad61d-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="ad61d-133">לדוגמה: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="ad61d-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="ad61d-134">לקבלת בעיות נפוצות ברישום המכשירים של תכלת Active Directory, ראה [שאלות נפוצות אודות מכשירים](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="ad61d-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
