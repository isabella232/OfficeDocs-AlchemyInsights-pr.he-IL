---
title: Active Directory אינו מסנכרן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265197"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e4d28-102">Active Directory אינו מסנכרן</span><span class="sxs-lookup"><span data-stu-id="e4d28-102">Active Directory not syncing</span></span>

<span data-ttu-id="e4d28-103">אם אתה מקבל שגיאות סינכרון, כגון "ללא סנכרון עדכני", או שים לב שמצב סינכרון הספריות בפורטל הניהול של Office אומר: "הסינכרון האחרון לפני יותר מ-3 ימים", יתכן כי AADConnect יש הגדרות שגויות או לא מספיקות הרשאות לביצוע סינכרון.</span><span class="sxs-lookup"><span data-stu-id="e4d28-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e4d28-104">התקנה מחדש של AADConnect באמצעות הגדרות מהירות עשויה לפתור את הבעיה במהירות:</span><span class="sxs-lookup"><span data-stu-id="e4d28-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="e4d28-105">[הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="e4d28-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e4d28-106">[בצע את ההוראות עבור התקנה מפורשת](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e4d28-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e4d28-107">לקבלת מידע נוסף על AADConnect חשבונות שירות, ראה [תכלת התחברות: חשבונות והרשאות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e4d28-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
