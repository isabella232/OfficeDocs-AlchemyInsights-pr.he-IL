---
title: בעיות בהסכמה למנהלי מערכת
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901130"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="e5e37-102">בעיות בהסכמה למנהלי מערכת</span><span class="sxs-lookup"><span data-stu-id="e5e37-102">Admin consent issues</span></span>

1. <span data-ttu-id="e5e37-103">הפוך את [זרימת העבודה להסכמה של מנהל](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) מערכת לזמינה כדי לאפשר למשתמשים לבקש אישור מנהל מערכת ישירות מהמסך ההסכמה.</span><span class="sxs-lookup"><span data-stu-id="e5e37-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="e5e37-104">אם אתה או משתמשי היישום שלך רואים שגיאות בלתי צפויות במהלך ההסכמה, עיין במאמר זה לקבלת שלבי פתרון בעיות: [שגיאה בלתי צפויה בעת ביצוע הסכמה ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="e5e37-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="e5e37-105">קבל מידע נוסף על [הסכמה למנהלי מערכת בפלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), כיצד פועלת [ההנחיה להסכמה](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) וכיצד [להעריך בקשה להסכמה למנהלי מערכת של הדיירים](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="e5e37-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="e5e37-106">יישומים המשולבים בפלטפורמת הזהויות של Microsoft ממלאים אחר מודל הרשאה המעניק למשתמשים ולשליטה באופן שבו ניתן לגשת לנתונים.</span><span class="sxs-lookup"><span data-stu-id="e5e37-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="e5e37-107">היישום של מודל ההרשאות עודכן בנקודת הקצה של פלטפורמת הזהות של Microsoft, והוא משנה את אופן הפעולה של האפליקציה עם פלטפורמת הזהות של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e5e37-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="e5e37-108">ראה [הרשאות והסכמה בנקודת הקצה של פלטפורמת הזהות של Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) לקבלת מבט כולל על מודל הרשאה זה, כולל טווחים, הרשאות והסכמה.</span><span class="sxs-lookup"><span data-stu-id="e5e37-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>