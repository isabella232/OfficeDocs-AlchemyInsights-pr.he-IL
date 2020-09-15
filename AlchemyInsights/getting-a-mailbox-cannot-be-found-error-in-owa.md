---
title: 126 אין אפשרות למצוא תיבת דואר ב-OWA?
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
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706751"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="e6876-102">מקבל שגיאת תיבת דואר לא נמצא ב-Outlook באינטרנט?</span><span class="sxs-lookup"><span data-stu-id="e6876-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="e6876-103">אם אתה משתמש ב-Outlook באינטרנט ואתה מקבל את **תיבת הדואר לא היתה אפשרות למצוא** שגיאה, החשבון שבו השתמשת כדי להתחבר ל-Outlook באינטרנט אינו כולל רשיון של Exchange Online ולכן אף תיבת דואר אינה משויכת לחשבון.</span><span class="sxs-lookup"><span data-stu-id="e6876-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="e6876-104">מנהל המערכת יכול להקצות רשיון לחשבון שלך על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e6876-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="e6876-105">פתח את [מרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/homepage) ועבור אל **משתמשים פעילים** תחת המקטע **משתמשים** ובחר את המשתמש הרואה את השגיאה.</span><span class="sxs-lookup"><span data-stu-id="e6876-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="e6876-106">בדף המשתמש שנפתח, עבור אל המקטע **רשיונות ויישומים** , בחר את ערך **המיקום** המתאים והקצה רשיון המכיל את Exchange Online (הרחב את הרשיון כדי לראות את הפרטים שלו).</span><span class="sxs-lookup"><span data-stu-id="e6876-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="e6876-107">לאחר שתסיים, לחץ על **שמור שינויים**.</span><span class="sxs-lookup"><span data-stu-id="e6876-107">When you're finished, click **Save changes**.</span></span>
