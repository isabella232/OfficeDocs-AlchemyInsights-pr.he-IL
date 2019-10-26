---
title: גישה מותנית עם Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504995"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="08327-102">גישה מותנית עם Intune</span><span class="sxs-lookup"><span data-stu-id="08327-102">Conditional Access with Intune</span></span>

<span data-ttu-id="08327-103">שימוש **בגישה מותנית** עם Intune דורש 3 שלבים:</span><span class="sxs-lookup"><span data-stu-id="08327-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="08327-104">צור **מדיניות גישה מותנית** המגדירה אילו משאבים מוגנים ואילו תנאים יש להכיר כדי לגשת למשאבים אלה.</span><span class="sxs-lookup"><span data-stu-id="08327-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="08327-105">לדוגמה, על התקן להיות תואם לפני הגישה לדואר אלקטרוני של חברה.</span><span class="sxs-lookup"><span data-stu-id="08327-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="08327-106">צור **מדיניות תאימות** כדי להגדיר הגדרות שחייבות להיות מולאו לפני שההתקן נחשב לתואם.</span><span class="sxs-lookup"><span data-stu-id="08327-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="08327-107">לדוגמה, על התקן להיות בעל pin של 6 ספרות לפחות לפני שהוא נחשב לתואם.</span><span class="sxs-lookup"><span data-stu-id="08327-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="08327-108">הבטחת הן **מדיניות תאימות** והן **פריטי מדיניות גישה מותנית** מיועדים לקבוצות המשתמשים הרצויות.</span><span class="sxs-lookup"><span data-stu-id="08327-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="08327-109">הדבר עשוי לדרוש יצירת קבוצות מסוימות של משתמשים בספריית הפעילות התכלת.</span><span class="sxs-lookup"><span data-stu-id="08327-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="08327-110">קרא עוד:</span><span class="sxs-lookup"><span data-stu-id="08327-110">Read more:</span></span>
  
- [<span data-ttu-id="08327-111">שיטות עבודה מומלצות לגישה מותנית</span><span class="sxs-lookup"><span data-stu-id="08327-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="08327-112">תחילת ההתחלה עם גישה מותנית</span><span class="sxs-lookup"><span data-stu-id="08327-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

