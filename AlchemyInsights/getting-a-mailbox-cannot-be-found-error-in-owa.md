---
title: 126 לא ניתן למצוא שגיאת קבלת תיבת דואר ב- OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426663"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="45abd-102">קבלת תיבת דואר לא נמצאה שגיאה ב- Outlook באינטרנט?</span><span class="sxs-lookup"><span data-stu-id="45abd-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="45abd-103">אם אתה משתמש ב- Outlook באינטרנט  ואתה מקבל תיבת דואר לא נמצאה לשגיאה, החשבון ששימש אותך להתחברות ל- Outlook באינטרנט אינו כולל רשיון Exchange Online ולכן, לא משויכת תיבת דואר לחשבון.</span><span class="sxs-lookup"><span data-stu-id="45abd-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="45abd-104">מנהל המערכת יכול להקצות רשיון לחשבון שלך על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="45abd-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="45abd-105">פתח את [מרכז הניהול של Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) עבור אל משתמשים פעילים תחת המקטע משתמשים ובחר את המשתמש ש רואה את השגיאה.  </span><span class="sxs-lookup"><span data-stu-id="45abd-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="45abd-106">בדף המשתמש שנפתח, עבור אל  המקטע רשיונות ואפליקציות,  בחר את ערך המיקום המתאים והקצה רשיון המכיל את Exchange Online (הרחב את הרשיון כדי לראות את הפרטים שלו).</span><span class="sxs-lookup"><span data-stu-id="45abd-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="45abd-107">כשתסיים, לחץ על **שמור שינויים.**</span><span class="sxs-lookup"><span data-stu-id="45abd-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="45abd-108">במקרים מסוימים, אם הרשיון כבר מוקצה לחשבון משתמש, הסרה והקצאה מחדש של הרשיון עוזרת לפתור את הבעיה ולהקצה אותה כראוי למערכת:</span><span class="sxs-lookup"><span data-stu-id="45abd-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="45abd-109">בדוק אם מנויי M365 Exchange Online (ועוד, אם יש לך) מנויים עדכניים ולא פג תוקף לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="45abd-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="45abd-110">לאחר שנוודא שתוקף המנוי שלך לא פג ורשיון חוקי הוקצה לחשבון המשתמש, ייתכן שהרשיון ימתין עד 24 שעות, ולכן ייתכן שיהיה עליך להמתין עד שהבעיה תיפתר.</span><span class="sxs-lookup"><span data-stu-id="45abd-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="45abd-111">לקבלת מידע נוסף, ראה [הקצאה וניהול של רשיונות](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="45abd-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>