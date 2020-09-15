---
title: Active Directory אינו מסתנכרן
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697630"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="60ab2-102">Active Directory אינו מסתנכרן</span><span class="sxs-lookup"><span data-stu-id="60ab2-102">Active Directory not syncing</span></span>

<span data-ttu-id="60ab2-103">אם אתה מקבל שגיאות סינכרון, כגון "ללא סינכרון אחרון", או להבחין במצב סינכרון מדריכי כתובות בפורטל מנהל המערכת של Office, מופיעה ההודעה "סינכרון אחרון של יותר מ-3 ימים", ייתכן שAADConnect יש הגדרות שגויות או הרשאות לא מספיקות לביצוע סינכרון.</span><span class="sxs-lookup"><span data-stu-id="60ab2-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="60ab2-104">התקנה מחדש של AADConnect באמצעות הגדרות אקספרס עשויה לפתור את הבעיה במהירות:</span><span class="sxs-lookup"><span data-stu-id="60ab2-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="60ab2-105">[הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="60ab2-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="60ab2-106">[בצע את ההוראות להתקנה מהירה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="60ab2-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="60ab2-107">לקבלת מידע נוסף אודות חשבונות שירות של AADConnect, ראה [התחברות והרשאות בנושא תכלת לספירה: חשבונות והרשאות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="60ab2-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
