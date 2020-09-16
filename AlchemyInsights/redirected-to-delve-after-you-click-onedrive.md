---
title: OneDrive for Business Web OneDrive מנתבת מחדש ל-התעמק
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776380"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="8c6c9-102">הופנה מחדש ל-OneDrive לאחר שתלחץ על</span><span class="sxs-lookup"><span data-stu-id="8c6c9-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="8c6c9-103">עיין [במדריך לפתרון בעיות](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)מפורט.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="8c6c9-104">כדי לפתור בעיה זו, מנהל המערכת חייב להעניק למשתמשים את הזכות ליצור את האתר ' האתרים שלי '.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="8c6c9-105">הסיבה לכך היא שדף OneDrive for Business נוצר באתרים שלי.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="8c6c9-106">כדי להעניק לזכות זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="8c6c9-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="8c6c9-107">במרכז הניהול של SharePoint, לחץ על **פרופילי משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="8c6c9-108">במקטע **אנשים** , לחץ על **ניהול הרשאות משתמש**.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="8c6c9-109">הוסף משתמשים הדורשים הרשאות ליצירת אתר האתרים שלי.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="8c6c9-110">כברירת מחדל, הגדרה זו מוגדרת **לכולם למעט משתמשים חיצוניים**.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="8c6c9-111">לאחר שהוספת את המשתמש, המשתמשים או הקבוצה, ודא שהאפשרות משתמש, משתמשים או הקבוצה שנוספה נבחרה, גלול אל המקטע **הרשאות** ולאחר מכן בחר את תיבת הסימון לצד **צור אתר אישי (נדרש עבור אחסון אישי, הזנה חדשותית ותוכן מופעל)**.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="8c6c9-112">לחץ על **אישור**, ולאחר מכן השתמש באפשרות ' נווט אל דף OneDrive ' כדי ליצור את האתר.</span><span class="sxs-lookup"><span data-stu-id="8c6c9-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
