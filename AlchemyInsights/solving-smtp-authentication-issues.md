---
title: הפיכת אימות SMTP לזמין ופתרון בעיות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077652"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="b1171-102">הפיכת אימות SMTP לזמין ופתרון בעיות</span><span class="sxs-lookup"><span data-stu-id="b1171-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="b1171-103">אם ברצונך להפוך אימות SMTP לזמין עבור תיבת דואר או אם אתה מקבל שגיאת "לקוח לא מאומת", "Authentication unsuccessful", או "SmtpClientAuthentication" עם קוד 5.7.57 או 5.7.3 או 5.7.139 בעת ניסיון להעביר דואר אלקטרוני על-ידי אימות מכשיר או יישום עם Microsoft 365, בצע שלוש פעולות אלה כדי לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="b1171-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="b1171-104">הפוך את [ברירות המחדל של אבטחה של Azure ללא](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) זמינות על-ידי הפעלת **ברירות מחדל של אבטחה** **ללא**.</span><span class="sxs-lookup"><span data-stu-id="b1171-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="b1171-105">a.</span><span class="sxs-lookup"><span data-stu-id="b1171-105">a.</span></span> <span data-ttu-id="b1171-106">היכנס לפורטל Azure כמנהל מערכת של אבטחה, כמנהל מערכת Access כללי או כמנהל מערכת כללי.</span><span class="sxs-lookup"><span data-stu-id="b1171-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="b1171-107">ב.</span><span class="sxs-lookup"><span data-stu-id="b1171-107">b.</span></span> <span data-ttu-id="b1171-108">עבור אל Azure Active Directory > **מאפיינים.**</span><span class="sxs-lookup"><span data-stu-id="b1171-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="b1171-109">c.</span><span class="sxs-lookup"><span data-stu-id="b1171-109">c.</span></span> <span data-ttu-id="b1171-110">בחר **ניהול ברירות מחדל של אבטחה**.</span><span class="sxs-lookup"><span data-stu-id="b1171-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="b1171-111">d.</span><span class="sxs-lookup"><span data-stu-id="b1171-111">d.</span></span> <span data-ttu-id="b1171-112">הגדר **את האפשרות הפוך ברירות מחדל של אבטחה לזמינות** **ללא**.</span><span class="sxs-lookup"><span data-stu-id="b1171-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="b1171-113">e.</span><span class="sxs-lookup"><span data-stu-id="b1171-113">e.</span></span> <span data-ttu-id="b1171-114">לחץ **שמור**.</span><span class="sxs-lookup"><span data-stu-id="b1171-114">Select **Save**.</span></span>

2. <span data-ttu-id="b1171-115">[הפוך הגשת SMTP של לקוח](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) לזמינה בתיבת הדואר המרשית.</span><span class="sxs-lookup"><span data-stu-id="b1171-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="b1171-116">a.</span><span class="sxs-lookup"><span data-stu-id="b1171-116">a.</span></span> <span data-ttu-id="b1171-117">מתוך מרכז הניהול של Microsoft 365, עבור אל **משתמשים פעילים** ובחר את המשתמש.</span><span class="sxs-lookup"><span data-stu-id="b1171-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="b1171-118">ב.</span><span class="sxs-lookup"><span data-stu-id="b1171-118">b.</span></span> <span data-ttu-id="b1171-119">עבור אל הכרטיסיה דואר ותחת יישומי **דואר אלקטרוני**, בחר ניהול יישומי **דואר אלקטרוני**.</span><span class="sxs-lookup"><span data-stu-id="b1171-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="b1171-120">d.</span><span class="sxs-lookup"><span data-stu-id="b1171-120">d.</span></span> <span data-ttu-id="b1171-121">ודא **שה- SMTP מאומת** נבחר (זמין).</span><span class="sxs-lookup"><span data-stu-id="b1171-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="b1171-122">e.</span><span class="sxs-lookup"><span data-stu-id="b1171-122">e.</span></span> <span data-ttu-id="b1171-123">בחר **שמור שינויים**.</span><span class="sxs-lookup"><span data-stu-id="b1171-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="b1171-124">[הפוך אימות רב-גורמי (MFA) ללא זמין](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) בתיבת הדואר המרשית.</span><span class="sxs-lookup"><span data-stu-id="b1171-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="b1171-125">a.</span><span class="sxs-lookup"><span data-stu-id="b1171-125">a.</span></span> <span data-ttu-id="b1171-126">עבור אל מרכז הניהול של Microsoft 365, ובתפריט הניווט הימני, בחר משתמשים   >  **פעילים משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="b1171-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="b1171-127">ב.</span><span class="sxs-lookup"><span data-stu-id="b1171-127">b.</span></span> <span data-ttu-id="b1171-128">בחר **אימות רב-גורמי**.</span><span class="sxs-lookup"><span data-stu-id="b1171-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="b1171-129">c.</span><span class="sxs-lookup"><span data-stu-id="b1171-129">c.</span></span> <span data-ttu-id="b1171-130">בחר את המשתמש והפוך את **אימות Multi-Factor ללא זמין.**</span><span class="sxs-lookup"><span data-stu-id="b1171-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
