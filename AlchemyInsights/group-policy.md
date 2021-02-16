---
title: מדיניות קבוצתית
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256777"
---
# <a name="group-policy"></a><span data-ttu-id="17467-102">מדיניות קבוצתית</span><span class="sxs-lookup"><span data-stu-id="17467-102">Group policy</span></span>

<span data-ttu-id="17467-103">הגדרות עבור אובייקטי משתמשים ומחשבים ב-תכלת Active Directory Domain Services (תכלת AD DS) מנוהלות לעתים קרובות באמצעות אובייקטי מדיניות קבוצתית (Gpo).</span><span class="sxs-lookup"><span data-stu-id="17467-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="17467-104">תכלת AD DS כולל אובייקטי Gpo מוכללים עבור משתמשי AADDC ומיכלי AADDC של מחשבים.</span><span class="sxs-lookup"><span data-stu-id="17467-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="17467-105">באפשרותך להתאים אישית אובייקטי Gpo מוכללים אלה כדי לקבוע תצורה של מדיניות קבוצתית לפי הצורך עבור הסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="17467-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="17467-106">לחברים בקבוצת מנהלי המערכת של תכלת לספירה יש הרשאות של ניהול מדיניות קבוצתית בתחום תכלת AD DS, וניתן גם ליצור אובייקטי Gpo ויחידות ארגוניות מותאמות אישית (Ou).</span><span class="sxs-lookup"><span data-stu-id="17467-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="17467-107">לקבלת מידע נוסף אודות המדיניות הקבוצתית ואופן הפעולה שלה, ראה [מבט כולל על מדיניות קבוצתית](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="17467-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="17467-108">בסביבה היברידית, פריטי מדיניות קבוצתית שתצורתם נקבעה בסביבת AD DS מקומית אינם מסונכרנים עם התכלת AD DS.</span><span class="sxs-lookup"><span data-stu-id="17467-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="17467-109">כדי להגדיר הגדרות תצורה עבור משתמשים או מחשבים ב-תכלת AD DS, ערוך אחד מאובייקטי ה-Gpo המהווים ברירת מחדל או צור GPO מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="17467-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="17467-110">מאמר זה [ניהול מדיניות קבוצתית](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) מראה לך כיצד להתקין את כלי ניהול המדיניות הקבוצתית, כיצד טון לערוך את אובייקטי ה-gpo המוכללים וכיצד ליצור אובייקטי gpo מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="17467-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



