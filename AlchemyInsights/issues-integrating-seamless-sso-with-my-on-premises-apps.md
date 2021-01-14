---
title: בעיות בשילוב של SSO חלק באמצעות היישומים המקומיים שלי
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868678"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="da0a5-102">בעיות בשילוב של SSO חלק באמצעות היישומים המקומיים שלי</span><span class="sxs-lookup"><span data-stu-id="da0a5-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="da0a5-103">כדי לפתור בעיות בשילוב של SSO חלק עם יישומים מקומיים, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="da0a5-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="da0a5-104">**שלבים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="da0a5-104">**Recommended steps**</span></span>

1. <span data-ttu-id="da0a5-105">כדי לקבוע תצורה של **יישום מקומי** עבור **כניסה יחידה באמצעות proxy של יישום**, ראה [מקומר סיסמה עבור כניסה יחידה באמצעות proxy של יישומים](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="da0a5-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="da0a5-106">**פתרון בעיות של Proxy של יישומים**: מומלץ להתחיל בסקירת זרימת פתרון [הבעיות, בעיות במחברי Proxy של יישומי proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), כדי לקבוע אם מחברי proxy של יישום מוגדרים כראוי.</span><span class="sxs-lookup"><span data-stu-id="da0a5-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="da0a5-107">אם אתה עדיין נתקל בבעיות בהתחברות ליישום, בצע את שלבי פתרון [הבעיות בנושא בעיות ביישום Proxy של יישומי Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="da0a5-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="da0a5-108">באפשרותך [לזהות בעיות](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ב-CORS באמצעות כלי איתור הבאגים הבאים של הדפדפן:</span><span class="sxs-lookup"><span data-stu-id="da0a5-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="da0a5-109">הפעל את הדפדפן ואתר את יישום האינטרנט.</span><span class="sxs-lookup"><span data-stu-id="da0a5-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="da0a5-110">הקש **F12** כדי להעלות את מסוף איתור הבאגים.</span><span class="sxs-lookup"><span data-stu-id="da0a5-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="da0a5-111">נסה לשחזר את הטרנזקציה וסקור את הודעת המסוף.</span><span class="sxs-lookup"><span data-stu-id="da0a5-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="da0a5-112">הפרה של CORS מפיקה שגיאת מסוף לגבי המקור.</span><span class="sxs-lookup"><span data-stu-id="da0a5-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="da0a5-113">לא ניתן לפתור בעיות מסוימות ב-CORS, כגון כאשר האפליקציה מנתבת מחדש ל-login.microsoftonline.com כדי לבצע אימות, והאסימון של access פג.</span><span class="sxs-lookup"><span data-stu-id="da0a5-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="da0a5-114">לאחר מכן, השיחה של CORS נכשלת.</span><span class="sxs-lookup"><span data-stu-id="da0a5-114">The CORS call then fails.</span></span> <span data-ttu-id="da0a5-115">פתרון עבור תרחיש זה הוא להאריך את משך החיים של אסימון הגישה, כדי למנוע ממנו לפוג במהלך הפעלת משתמש.</span><span class="sxs-lookup"><span data-stu-id="da0a5-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="da0a5-116">לקבלת מידע נוסף אודות האופן שבו ניתן לעשות זאת, ראה [אורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="da0a5-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="da0a5-117">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="da0a5-117">**Recommended documents**</span></span>

- [<span data-ttu-id="da0a5-118">כיצד להגדיר כניסה יחידה ליישום Proxy של יישום</span><span class="sxs-lookup"><span data-stu-id="da0a5-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="da0a5-119">SAML כניסה יחידה עבור יישומים מקומיים עם Proxy של יישומים</span><span class="sxs-lookup"><span data-stu-id="da0a5-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="da0a5-120">הכרת בעיות ביישום Proxy של יישום מדריך כתובות של Active Directory CORS</span><span class="sxs-lookup"><span data-stu-id="da0a5-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="da0a5-121">פתרון בעיות של תצורות הקצאה מוגבלת של Kerberos עבור Proxy של יישומים</span><span class="sxs-lookup"><span data-stu-id="da0a5-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)