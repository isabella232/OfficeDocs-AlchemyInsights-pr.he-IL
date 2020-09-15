---
title: שגיאת teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700204"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="fe0e6-102">שגיאה של 4c7 ב-Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fe0e6-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="fe0e6-103">שגיאה זו מתרחשת מאחר ש-Microsoft Teams דורש אימות טפסים.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="fe0e6-104">בעת פריסת שירותי האיחוד של Active Directory (AD FS), אימות טפסים אינו זמין עבור האינטרא כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="fe0e6-105">אם האימות המשולב של Windows נכשל, אתה מתבקש להיכנס באמצעות אימות טפסים.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="fe0e6-106">כדי לפתור בעיה זו, אפשר אימות טפסים באמצעות יישום ה-snap-in של מסוף הניהול של AD FS (MMC) במחשב שבו מותקן העותק המקומי של Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="fe0e6-107">לשם כך, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="fe0e6-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="fe0e6-108">בחלונית הניווט, אתר את **מדיניות האימות**.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="fe0e6-109">תחת **פעולות** בחלונית הפרטים, בחר **ערוך אימות ראשי כללי**.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="fe0e6-110">בכרטיסיה **אינטרא-נט** , בחר **אימות טפסים**.</span><span class="sxs-lookup"><span data-stu-id="fe0e6-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="fe0e6-111">בחר **אישור** (או **החל**).</span><span class="sxs-lookup"><span data-stu-id="fe0e6-111">Select **OK** (or **Apply**).</span></span>