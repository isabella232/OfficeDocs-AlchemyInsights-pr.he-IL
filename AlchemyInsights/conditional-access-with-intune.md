---
title: Access מותנה עם Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935938"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b8a33-102">Access מותנה עם Intune</span><span class="sxs-lookup"><span data-stu-id="b8a33-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b8a33-103">באמצעות **Access מותנה** Intune דורש 3 שלבים:</span><span class="sxs-lookup"><span data-stu-id="b8a33-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="b8a33-p101">יצירת **מדיניות Access מותנה** המגדיר המוגן אילו משאבים, ואת התנאים הדרושים יתקיימו לקבל גישה למשאבים אלה. לדוגמה, התקן חייב להיות תואם בטרם ניגש דוא של החברה.</span><span class="sxs-lookup"><span data-stu-id="b8a33-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="b8a33-p102">יצירת **מדיניות תאימות** כדי להגדיר הגדרות שיש לעמוד בהן לפני נחשבת להתקן תואם. לדוגמה, התקן חייב להיות ה-pin של ספרות לפחות 6 לפני שהיא נחשבת תואם.</span><span class="sxs-lookup"><span data-stu-id="b8a33-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="b8a33-p103">הבטחת **תאימות מדיניות** **ומדיניות Access מותנה** מיועדים לקבוצות הרצוי של משתמשים. פעולה זו עשויה לדרוש יצירת קבוצות מסוימות של משתמשים ב- Active Directory תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="b8a33-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="b8a33-110">קרא עוד:</span><span class="sxs-lookup"><span data-stu-id="b8a33-110">Read more:</span></span>
  
- [<span data-ttu-id="b8a33-111">מותנה Access, שיטות עבודה מומלצות</span><span class="sxs-lookup"><span data-stu-id="b8a33-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="b8a33-112">תחילת העבודה עם Access מותנה</span><span class="sxs-lookup"><span data-stu-id="b8a33-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

