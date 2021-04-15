---
title: שגיאת Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786670"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="58f24-102">שגיאת 4c7 ב- Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="58f24-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="58f24-103">שגיאה זו מתרחשת מאחר ש- Microsoft Teams דורש אימות טפסים.</span><span class="sxs-lookup"><span data-stu-id="58f24-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="58f24-104">בעת פריסת Active Directory Federation Services (AD FS), אימות טפסים אינו זמין עבור האינטרא-נט כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="58f24-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="58f24-105">אם האימות המשולב של Windows נכשל, תתבקש להיכנס באמצעות אימות טפסים.</span><span class="sxs-lookup"><span data-stu-id="58f24-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="58f24-106">כדי לפתור בעיה זו, הפוך אימות טפסים לזמין באמצעות יישום ה- Snap-in AD FS Microsoft Management Console (MMC) במחשב המכיל את העותק המקומי של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="58f24-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="58f24-107">לשם כך, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="58f24-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="58f24-108">בחלונית הניווט, עבור אל **מדיניות אימות**.</span><span class="sxs-lookup"><span data-stu-id="58f24-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="58f24-109">תחת **פעולות** בחלונית הפרטים, בחר **ערוך אימות ראשי כללי.**</span><span class="sxs-lookup"><span data-stu-id="58f24-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="58f24-110">בכרטיסיה **אינטרא-נט,** בחר **אימות טפסים**.</span><span class="sxs-lookup"><span data-stu-id="58f24-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="58f24-111">בחר **אישור** (או **החל).**</span><span class="sxs-lookup"><span data-stu-id="58f24-111">Select **OK** (or **Apply**).</span></span>