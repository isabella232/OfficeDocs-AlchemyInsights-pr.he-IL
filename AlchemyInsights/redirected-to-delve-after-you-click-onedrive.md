---
title: OneDrive for Business Web OneDrive מנותב מחדש אל Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799990"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="25382-102">מנותב מחדש ל- Delve לאחר לחיצה על OneDrive</span><span class="sxs-lookup"><span data-stu-id="25382-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="25382-103">עיין במדריך מפורט [לפתרון בעיות](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="25382-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="25382-104">כדי לפתור בעיה זו, מנהל המערכת חייב להעניק למשתמשים את הזכות ליצור את האתר 'האתרים שלי' שלו.</span><span class="sxs-lookup"><span data-stu-id="25382-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="25382-105">זאת משום שהדף OneDrive for Business נוצר באתרים שלי.</span><span class="sxs-lookup"><span data-stu-id="25382-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="25382-106">כדי להעניק זכות זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="25382-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="25382-107">במרכז הניהול של SharePoint, לחץ על **פרופילי משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="25382-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="25382-108">במקטע **אנשים,** לחץ על **ניהול הרשאות משתמש**.</span><span class="sxs-lookup"><span data-stu-id="25382-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="25382-109">הוסף משתמשים הדורשים הרשאות כדי ליצור את אתר האתרים שלי שלהם.</span><span class="sxs-lookup"><span data-stu-id="25382-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="25382-110">כברירת מחדל, הגדרה זו מוגדרת לכולם **למעט משתמשים חיצוניים.**</span><span class="sxs-lookup"><span data-stu-id="25382-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="25382-111">לאחר הוספת המשתמש, המשתמשים או הקבוצה, ודא שהמשתמש, המשתמשים או הקבוצה שנוספו  נבחרו, גלול למקטע ההרשאות ולאחר מכן בחר את תיבת הסימון לצד יצירת אתר אישי (נדרש עבור אחסון אישי, הזנה חדשותית **ותוכן עוקב)**.</span><span class="sxs-lookup"><span data-stu-id="25382-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="25382-112">לחץ **על** אישור ולאחר מכן תעיין בדף OneDrive כדי ליצור את האתר.</span><span class="sxs-lookup"><span data-stu-id="25382-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
