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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504995"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9badc-102">Access מותנה עם Intune</span><span class="sxs-lookup"><span data-stu-id="9badc-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9badc-103">באמצעות **Access מותנה** Intune דורש 3 שלבים:</span><span class="sxs-lookup"><span data-stu-id="9badc-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="9badc-104">יצירת **מדיניות Access מותנה** המגדיר המוגן אילו משאבים, ואת התנאים הדרושים יתקיימו לקבל גישה למשאבים אלה.</span><span class="sxs-lookup"><span data-stu-id="9badc-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="9badc-105">לדוגמה, התקן חייב להיות תואם בטרם ניגש דוא של החברה.</span><span class="sxs-lookup"><span data-stu-id="9badc-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="9badc-106">יצירת **מדיניות תאימות** כדי להגדיר הגדרות שיש לעמוד בהן לפני נחשבת להתקן תואם.</span><span class="sxs-lookup"><span data-stu-id="9badc-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9badc-107">לדוגמה, התקן חייב להיות ה-pin של ספרות לפחות 6 לפני שהיא נחשבת תואם.</span><span class="sxs-lookup"><span data-stu-id="9badc-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="9badc-108">הבטחת **תאימות מדיניות** **ומדיניות Access מותנה** מיועדים לקבוצות הרצוי של משתמשים.</span><span class="sxs-lookup"><span data-stu-id="9badc-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="9badc-109">פעולה זו עשויה לדרוש יצירת קבוצות מסוימות של משתמשים ב- Active Directory תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="9badc-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="9badc-110">קרא עוד:</span><span class="sxs-lookup"><span data-stu-id="9badc-110">Read more:</span></span>
  
- [<span data-ttu-id="9badc-111">מותנה Access, שיטות עבודה מומלצות</span><span class="sxs-lookup"><span data-stu-id="9badc-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="9badc-112">תחילת העבודה עם Access מותנה</span><span class="sxs-lookup"><span data-stu-id="9badc-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

