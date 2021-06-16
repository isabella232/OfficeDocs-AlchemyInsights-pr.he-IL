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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930976"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="6c6dc-102">Active Directory אינו מסתנכרן</span><span class="sxs-lookup"><span data-stu-id="6c6dc-102">Active Directory not syncing</span></span>

<span data-ttu-id="6c6dc-103">אם אתה מקבל שגיאות סינכרון, כגון "ללא סינכרון לאחרונה", או שים לב למצב סינכרון מדריכי הכתובות בפורטל הניהול של Office רשום "הסינכרון האחרון לפני יותר מ- 3 ימים", ייתכן של- AADConnect יש הגדרות שגויות או הרשאות לא מספיקות לביצוע סינכרון.</span><span class="sxs-lookup"><span data-stu-id="6c6dc-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="6c6dc-104">התקנה מחדש של AADConnect באמצעות הגדרות מהירות עשויה לפתור את הבעיה במהירות:</span><span class="sxs-lookup"><span data-stu-id="6c6dc-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="6c6dc-105">[הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="6c6dc-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="6c6dc-106">[בצע את ההוראות להתקנה מהירה.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="6c6dc-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="6c6dc-107">Azure AD Connect חייב להיות מותקן ב- Windows Server 2012 או גירסה מאוחרת יותר.</span><span class="sxs-lookup"><span data-stu-id="6c6dc-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="6c6dc-108">שרת זה חייב להיות מצורף לתחום והוא יכול להיות בקר תחום או שרת עמית.</span><span class="sxs-lookup"><span data-stu-id="6c6dc-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="6c6dc-109">לקבלת רשימה מלאה של דרישות התחברות של Azure AD ודרישות מוקדמות, עיין בדרישות מוקדמות עבור [Azure AD התחברות.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="6c6dc-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="6c6dc-110">לקבלת מידע נוסף אודות חשבונות שירות של AADConnect, ראה [Azure AD התחברות: חשבונות והרשאות](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="6c6dc-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
