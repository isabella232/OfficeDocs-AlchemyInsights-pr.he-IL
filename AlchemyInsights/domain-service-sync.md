---
title: סינכרון שירותי תחומים
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885156"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="23a7f-102">סינכרון שירותי תחומים</span><span class="sxs-lookup"><span data-stu-id="23a7f-102">Domain service synchronization</span></span>

<span data-ttu-id="23a7f-103">אובייקטים ואישורים בתחום הניהול של תכלת Active Directory (תכלת AD DS) יכולים להיווצר באופן מקומי בתוך התחום, או לסנכרן אותו מדייר תכלת Active Directory (תכלת לספירה).</span><span class="sxs-lookup"><span data-stu-id="23a7f-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="23a7f-104">כאשר אתה פורס לראשונה את התכלת AD DS, מוגדרת סינכרון חד-כיוון אוטומטי ומופעל כדי לשכפל את האובייקטים מ-תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="23a7f-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="23a7f-105">סינכרון חד-כיוון זה ממשיך לפעול ברקע כדי לשמור על העדכניות של התחום המנוהל ' תכלת AD DS ' עם כל השינויים שבוצעו במאמר תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="23a7f-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="23a7f-106">לא מופיע סינכרון מתכלת AD DS בחזרה לתכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="23a7f-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="23a7f-107">לקבלת פרטים נוספים על סינכרון שירות התחומים של תכלת Active Directory, ראה [סינכרון שירות תחום](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="23a7f-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
