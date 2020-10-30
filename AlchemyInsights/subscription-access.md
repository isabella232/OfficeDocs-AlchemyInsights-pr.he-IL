---
title: גישה למנוי
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807433"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="ecdb7-102">לא ניתן להיכנס לתכלת עקב בעיות בדפדפן (הדפדפן נתקע, ממשיך להסתובב, אינו נטען וכדומה).</span><span class="sxs-lookup"><span data-stu-id="ecdb7-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="ecdb7-103">ייתכן שאתה מושפע מהנפילה.</span><span class="sxs-lookup"><span data-stu-id="ecdb7-103">You might be impacted by an outage.</span></span> <span data-ttu-id="ecdb7-104">בדוק אם קיימת הפסקת פעולה מתמשכת: [מצבי תקינות התכלת](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="ecdb7-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="ecdb7-105">צא מכל ההפעלות הפעילות של ' תכלת '.</span><span class="sxs-lookup"><span data-stu-id="ecdb7-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="ecdb7-106">התחל מצב של דפדפן האינטרנט באופן פרטי או בעילום שם.</span><span class="sxs-lookup"><span data-stu-id="ecdb7-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="ecdb7-107">באפשרותך גם לנסות לרענן דפדפן, להשתמש בדפדפן אחר, למחוק קבצי cookie של מטמון אם לעיל אינו פועל.</span><span class="sxs-lookup"><span data-stu-id="ecdb7-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="ecdb7-108">מידע נוסף: [פתרון בעיות כניסה](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="ecdb7-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="ecdb7-109">**אין אפשרות לגשת למנויים**</span><span class="sxs-lookup"><span data-stu-id="ecdb7-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="ecdb7-110">בפורטל ' [תכלת](https://portal.azure.com/)', ודא שהאפשרות ' התכלת הנכון ' נבחרה מהחשבון בחלק השמאלי העליון.</span><span class="sxs-lookup"><span data-stu-id="ecdb7-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="ecdb7-111">במרכז [החשבון של תכלת](https://account.windowsazure.com/Subscriptions), ודא שהחשבון משמש כמנהל החשבון.</span><span class="sxs-lookup"><span data-stu-id="ecdb7-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="ecdb7-112">מידע נוסף: [פתרון בעיות לא נמצאו מנויים](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ecdb7-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="ecdb7-113">**לא ניתן לגשת להיסטוריית החיוב**</span><span class="sxs-lookup"><span data-stu-id="ecdb7-113">**Unable to access billing history**</span></span>

<span data-ttu-id="ecdb7-114">מנהל החשבונות צריך לוודא שהמשתמש הניגש לפרטי החיוב מתווסף ל-תכלת Active directory כמשתמש אורח: [הוספה או מחיקה של משתמש חדש](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ecdb7-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ecdb7-115">לאחר מכן, המשתמש צריך לקבל תפקיד מנהל מערכת כללי: [הקצה תפקיד למשתמשים](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ecdb7-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ecdb7-116">פרסם זאת, המשתמש יכול לקבל גישה לחיוב באמצעות מדיניות RBAC: [הענקת גישה לחיוב](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ecdb7-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ecdb7-117">**מסמכים מומלצים**</span><span class="sxs-lookup"><span data-stu-id="ecdb7-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="ecdb7-118">איני מצליח להיכנס כדי לנהל את מנוי התכלת שלי</span><span class="sxs-lookup"><span data-stu-id="ecdb7-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)