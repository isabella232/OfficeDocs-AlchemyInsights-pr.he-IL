---
title: שגיאה בצוותים 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796152"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="122c7-102">שגיאת 4c7 בצוותי Microsoft</span><span class="sxs-lookup"><span data-stu-id="122c7-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="122c7-103">שגיאה זו מתרחשת מאחר שצוותי Microsoft דורשים אימות טפסים.</span><span class="sxs-lookup"><span data-stu-id="122c7-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="122c7-104">בעת פריסת שירותי פדרציית הספריות של Active Directory (AD FS), אימות טפסים אינו מאופשר עבור האינטרא כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="122c7-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="122c7-105">אם האימות המשולב של Windows נכשל, תתבקש להיכנס באמצעות אימות טפסים.</span><span class="sxs-lookup"><span data-stu-id="122c7-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="122c7-106">כדי לפתור בעיה זו, הפוך את אימות הטפסים לזמין באמצעות יישום ה-snap-in של מסוף הניהול של Microsoft FS (MMC) במחשב המכיל את העותק המקומי של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="122c7-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="122c7-107">כדי לעשות זאת, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="122c7-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="122c7-108">בחלונית הניווט, דפדף אל **מדיניות אימות**.</span><span class="sxs-lookup"><span data-stu-id="122c7-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="122c7-109">תחת **פעולות** בחלונית הפרטים, בחר באפשרות **ערוך אימות ראשי כללי**.</span><span class="sxs-lookup"><span data-stu-id="122c7-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="122c7-110">בכרטיסיה **אינטרא-נט** , בחר באפשרות **אימות טפסים**.</span><span class="sxs-lookup"><span data-stu-id="122c7-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="122c7-111">בחר **ב'אישור '** (או **החל**).</span><span class="sxs-lookup"><span data-stu-id="122c7-111">Select **OK** (or **Apply**).</span></span>