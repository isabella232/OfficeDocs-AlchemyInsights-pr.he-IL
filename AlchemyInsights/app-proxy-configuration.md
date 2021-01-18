---
title: תצורת Proxy של יישום
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885133"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="e98e4-102">תצורת Proxy של יישום</span><span class="sxs-lookup"><span data-stu-id="e98e4-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="e98e4-103">כדי להבין כיצד לקבוע את התצורה של יישום Proxy של יישום בתוך ' תכלת לספירה ' כדי לחשוף את היישומים המקומיים שלך לענן, ראה [כיצד לקבוע את התצורה של יישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="e98e4-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="e98e4-104">כניסה יחידה (SSO) מאפשרת למשתמשים לגשת ליישום מבלי לאמת מספר פעמים.</span><span class="sxs-lookup"><span data-stu-id="e98e4-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="e98e4-105">היא מאפשרת לאימות בודד להתרחש בענן, כנגד תכלת Active Directory, ומאפשרת לשירות או למחבר להתחזות למשתמש להשלים את כל האתגרים הנוספים של אימות מהיישום.</span><span class="sxs-lookup"><span data-stu-id="e98e4-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="e98e4-106">לקבלת מידע נוסף, ראה [כיצד לקבוע את תצורת הכניסה היחידה ליישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="e98e4-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="e98e4-107">[השתמש במאמר זה](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) כדי לפתור בעיות נפוצות שאנשים מתמודדים בעת יצירת יישום proxy חדש של יישום.</span><span class="sxs-lookup"><span data-stu-id="e98e4-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="e98e4-108">אם אתה נתקל בבעיה בהגדרת אימות עורפי ליישום שלך, ייתכן שתצטרך [לפתור תצורות הקצאה מוגבלת של Kerberos עבור Proxy של יישומים](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) או לבצע הדרכה בנושא [קביעת התצורה של יישום עם PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) כדי לפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="e98e4-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
