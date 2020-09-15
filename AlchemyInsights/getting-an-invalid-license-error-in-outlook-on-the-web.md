---
title: 125 מקבל שגיאת רשיון לא חוקית ב-Outlook באינטרנט?
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 825d91cd81646767b100e6fc964d7a94b8bc6879
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677460"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a><span data-ttu-id="55c69-102">מקבל שגיאת רשיון לא חוקית ב-Outlook באינטרנט?</span><span class="sxs-lookup"><span data-stu-id="55c69-102">Getting an invalid license error in Outlook on the web?</span></span>

<span data-ttu-id="55c69-103">אם אתה משתמש ב-Outlook באינטרנט ואתה מקבל **משהו שגיאה שגויה** המכילה **X-OWA-שגיאה: Microsoft. Exchange. Data. InvalidLicenseException**, רשיון Exchange Online שלך אינו מוקצה כראוי או שפג תוקפו לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="55c69-103">If you're using Outlook on the web and you get a **Something went wrong** error that contains **X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException**, your Exchange Online license isn't correctly assigned or has recently expired.</span></span> <span data-ttu-id="55c69-104">מנהל המערכת יכול להקצות לך רשיון על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="55c69-104">Your admin can assign a license to you by following these steps:</span></span>
  
1. <span data-ttu-id="55c69-105">פתח את [מרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/homepage) ותחת **משתמשים פעילים**, בחר **ערוך משתמש**.</span><span class="sxs-lookup"><span data-stu-id="55c69-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="55c69-106">בדף **עריכת משתמש** שנפתח, בחר את המשתמש.</span><span class="sxs-lookup"><span data-stu-id="55c69-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="55c69-107">בדף ' מאפייני משתמש ' שנפתח, לחץ על **ערוך** עבור **רשיונות מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="55c69-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="55c69-108">בדף **רשיונות מוצר** שנפתח, בחר את ערך **המיקום** המתאים והקצה רשיון המכיל את Exchange Online (הרחב את הרשיון כדי לראות את הפרטים שלו).</span><span class="sxs-lookup"><span data-stu-id="55c69-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="55c69-109">לסיום, לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="55c69-109">When you're finished, click **Save**.</span></span>
