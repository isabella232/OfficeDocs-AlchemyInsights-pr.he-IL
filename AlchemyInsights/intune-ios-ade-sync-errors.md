---
title: שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448923"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="670f7-102">שגיאות סינכרון של הרשמת מכשירים אוטומטיות של Apple</span><span class="sxs-lookup"><span data-stu-id="670f7-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="670f7-103">"זיהינו שיש לך אסימון ADE/DEP אחד או יותר הנמצאים במצב שגיאה.</span><span class="sxs-lookup"><span data-stu-id="670f7-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="670f7-104">עד שמצב השגיאה ייפתר עבור כל אסימון מושפע, הפונקציונליות של ADE לא תפעל כמצופה.</span><span class="sxs-lookup"><span data-stu-id="670f7-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="670f7-105">שגיאה זו עשויה להופיע במספר דרכים, כולל:</span><span class="sxs-lookup"><span data-stu-id="670f7-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="670f7-106">המכשירים עשויים שלא להסתנכרן מ-ABM/ASM כדי לכוונן</span><span class="sxs-lookup"><span data-stu-id="670f7-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="670f7-107">הקצאות של פרופילי ההרשמה עשויות להיכשל</span><span class="sxs-lookup"><span data-stu-id="670f7-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="670f7-108">המכשירים עשויים שלא להשלים את ההרשמה של ADE בהצלחה</span><span class="sxs-lookup"><span data-stu-id="670f7-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="670f7-109">חפש את שגיאת הסינכרון המדווחת במסוף ה-intune תחת **מכשירים > התקני הרשמה > Apple הרשמת > אסימונים של תוכנית ההרשמה**.</span><span class="sxs-lookup"><span data-stu-id="670f7-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="670f7-110">אחת הסיבות הנפוצות ביותר לשגיאת סינכרון היא תפוגת האסימון הנוכחי.</span><span class="sxs-lookup"><span data-stu-id="670f7-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="670f7-111">במקרים רבים, חידוש האסימון המושפע יפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="670f7-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="670f7-112">אם פג תוקף אחד או יותר מהאסימונים שלך, עיין בתיעוד הבא כדי לעזור לך לחדש אותם באופן המתאים:</span><span class="sxs-lookup"><span data-stu-id="670f7-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="670f7-113">חידוש אסימון הרשמה אוטומטית של מכשירים</span><span class="sxs-lookup"><span data-stu-id="670f7-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="670f7-114">בנוסף, באפשרותך לראות את המסמכים הבאים כדי לראות תיקונים פוטנציאליים עבור שגיאות אחרות הגורמות לכשלים בסינכרון אסימונים:</span><span class="sxs-lookup"><span data-stu-id="670f7-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="670f7-115">שגיאות סינכרון של ABM/ASM for iOS/iPadOS ו-macOS להרשמת מכשירים אוטומטיים</span><span class="sxs-lookup"><span data-stu-id="670f7-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="670f7-116">שגיאות סינכרון של ABM/ASM for iOS/iPadOS ו-macOS להרשמת מכשירים אוטומטיים</span><span class="sxs-lookup"><span data-stu-id="670f7-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
