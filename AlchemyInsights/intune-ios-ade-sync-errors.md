---
title: שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714834"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="a0533-102">שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple</span><span class="sxs-lookup"><span data-stu-id="a0533-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="a0533-103">"זיהינו שיש לך אסימון ADE/DEP אחד או יותר הנמצאים במצב שגיאה.</span><span class="sxs-lookup"><span data-stu-id="a0533-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="a0533-104">עד שמצב השגיאה ייפתר עבור כל אסימון מושפע, הפונקציונליות של ADE לא תפעל באופן זהה ".</span><span class="sxs-lookup"><span data-stu-id="a0533-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="a0533-105">שגיאה זו עשויה להופיע במספר דרכים, כולל:</span><span class="sxs-lookup"><span data-stu-id="a0533-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="a0533-106">המכשירים עשויים שלא להסתנכרן מ-ABM/ASM כדי לכוונן</span><span class="sxs-lookup"><span data-stu-id="a0533-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="a0533-107">הקצאות של פרופילי ההרשמה עשויות להיכשל</span><span class="sxs-lookup"><span data-stu-id="a0533-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="a0533-108">המכשירים עשויים שלא להשלים את ההרשמה של ADE בהצלחה</span><span class="sxs-lookup"><span data-stu-id="a0533-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="a0533-109">חפש את שגיאת הסינכרון המדווחת במסוף ה-intune תחת **מכשירים > התקני הרשמה > Apple הרשמה > אסימונים** וסקור את המסמכים הבאים כדי לראות את כל התיקונים הפוטנציאליים:</span><span class="sxs-lookup"><span data-stu-id="a0533-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="a0533-110">שגיאות סינכרון של ABM/ASM for iOS/iPadOS ו-macOS להרשמת מכשירים אוטומטיים</span><span class="sxs-lookup"><span data-stu-id="a0533-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
