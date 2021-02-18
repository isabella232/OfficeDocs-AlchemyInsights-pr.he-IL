---
title: ניהול הגדרות חיצוניות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294319"
---
# <a name="managing-external-settings"></a><span data-ttu-id="f55b3-102">ניהול הגדרות חיצוניות</span><span class="sxs-lookup"><span data-stu-id="f55b3-102">Managing External Settings</span></span>

<span data-ttu-id="f55b3-103">**הכרזה**</span><span class="sxs-lookup"><span data-stu-id="f55b3-103">**Announcement**</span></span>

- <span data-ttu-id="f55b3-104">[תבטלות של תמיכה בכניסה של תצוגת האינטרנט מ-Google החל מ-4 בינואר 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="f55b3-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="f55b3-105">בדיקה אם היישומים שלך מושפעים על-ידי ביצוע ההדרכה של Google בנושא תאימות בדיקות</span><span class="sxs-lookup"><span data-stu-id="f55b3-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="f55b3-106">הקפד להשתמש בתצוגת האינטרנט של המערכת או בדפדפן המערכת בעת כניסה למשתמשים באמצעות חשבונות של Google לצרכן</span><span class="sxs-lookup"><span data-stu-id="f55b3-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="f55b3-107">**ניהול הגדרות הזמנה**</span><span class="sxs-lookup"><span data-stu-id="f55b3-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="f55b3-108">ודא [שהגדרת את הגדרות שיתוף הפעולה החיצוני](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) כדי לאפשר לאנשים המתאימים לשלוח הזמנות.</span><span class="sxs-lookup"><span data-stu-id="f55b3-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="f55b3-109">**ניהול הרשאות גישה של משתמשים אורחים**</span><span class="sxs-lookup"><span data-stu-id="f55b3-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="f55b3-110">מנהלי מערכת כלליים יכולים לנהל הרשאות של גישת אורח בספריה באמצעות הפורטל ' תכלת ' על-ידי קביעת התצורה של הרשאות גישת אורח בדף הגדרות שיתוף פעולה חיצוני.</span><span class="sxs-lookup"><span data-stu-id="f55b3-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="f55b3-111">[קבל מידע נוסף על הגדרה זו](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f55b3-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="f55b3-112">אם אתה מעוניין שהאורחים שלך יוכלו לגשת ליישומים כגון Teams או SharePoint, ודא שהגדרת יישומים אלה כדי לאפשר גישת אורח.</span><span class="sxs-lookup"><span data-stu-id="f55b3-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="f55b3-113">קבל מידע נוסף על [הגדרות teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) ו- [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f55b3-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f55b3-114">**הגדרת הזמנות:**</span><span class="sxs-lookup"><span data-stu-id="f55b3-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="f55b3-115">הפיכת שיתוף פעולה חיצוני של B2B לזמין וניהול מי יכול להזמין אורחים</span><span class="sxs-lookup"><span data-stu-id="f55b3-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f55b3-116">אפשר או חסום הזמנות למשתמשים מארגונים ספציפיים</span><span class="sxs-lookup"><span data-stu-id="f55b3-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="f55b3-117">**קביעת התצורה של ספקי הזהויות המותרים:**</span><span class="sxs-lookup"><span data-stu-id="f55b3-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="f55b3-118">הפדרציה של Google</span><span class="sxs-lookup"><span data-stu-id="f55b3-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f55b3-119">איגוד ישיר</span><span class="sxs-lookup"><span data-stu-id="f55b3-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f55b3-120">דואר אלקטרוני-אימות קוד סיסמה חד-פעמי</span><span class="sxs-lookup"><span data-stu-id="f55b3-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
