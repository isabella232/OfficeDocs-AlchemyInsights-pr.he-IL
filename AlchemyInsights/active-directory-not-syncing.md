---
title: Active Directory אינו מסתנכרן
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822852"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="c757b-102">Active Directory אינו מסתנכרן</span><span class="sxs-lookup"><span data-stu-id="c757b-102">Active Directory not syncing</span></span>

<span data-ttu-id="c757b-103">אם אתה מקבל שגיאות סינכרון, כגון "ללא סינכרון לאחרונה", או שים לב למצב סינכרון מדריכי הכתובות בפורטל הניהול של Office, "Last synced לפני יותר מ- 3 ימים", ייתכן של- AADConnect יש הגדרות שגויות או הרשאות לא מספיקות לביצוע סינכרון.</span><span class="sxs-lookup"><span data-stu-id="c757b-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="c757b-104">התקנה מחדש של AADConnect באמצעות הגדרות מהירות עשויה לפתור את הבעיה במהירות:</span><span class="sxs-lookup"><span data-stu-id="c757b-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="c757b-105">[הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="c757b-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="c757b-106">[בצע את ההוראות להתקנה מהירה.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="c757b-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="c757b-107">לקבלת מידע נוסף אודות חשבונות שירות של AADConnect, ראה [Azure AD Connect: חשבונות והרשאות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="c757b-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
