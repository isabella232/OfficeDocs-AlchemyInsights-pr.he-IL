---
title: 902 (שגיאות סינכרון עקב אובייקטים כפולים)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737342"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="36247-102">שגיאות סינכרון עקב אובייקטים כפולים</span><span class="sxs-lookup"><span data-stu-id="36247-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="36247-103">ייתכן שתקבל אחת מהודעות השגיאה הבאות כאשר סינכרון מדריכי כתובות מסתיים ב-Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="36247-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="36247-104">לא ניתן לעדכן אובייקט זה ב-Microsoft Online Services מאחר שהתכונות הבאות המשויכות לאובייקט זה מכילים ערכים שכבר משויכים לאובייקט אחר במדריך הכתובות המקומי שלך.</span><span class="sxs-lookup"><span data-stu-id="36247-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="36247-105">אובייקט מסונכרן עם אותה כתובת proxy קיים כבר במדריך הכתובות של Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="36247-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="36247-106">לא ניתן לעדכן אובייקט זה מאחר שהתכונות הבאות המשויכות לאובייקט זה מכילים ערכים שכבר משויכים לאובייקט אחר בשירותי מדריך הכתובות המקומי: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="36247-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="36247-107">כדי לזהות ולפתור את הבעיה, הורד והפעיל את [כלי התיקון של שגיאות IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="36247-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="36247-108">לקבלת מידע נוסף, ראה [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="36247-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
