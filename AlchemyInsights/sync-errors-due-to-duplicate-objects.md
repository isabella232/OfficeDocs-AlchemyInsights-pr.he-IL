---
title: 902 (שגיאות סינכרון עקב אובייקטים כפולים)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767128"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="1e061-102">שגיאות סינכרון עקב אובייקטים כפולים</span><span class="sxs-lookup"><span data-stu-id="1e061-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="1e061-103">ייתכן שתתקבל אחת מהודעות השגיאה הבאות כאשר סינכרון ספריות מסיים ב-Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="1e061-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="1e061-104">אין אפשרות לעדכן אובייקט זה ב-Microsoft Online Services מאחר שהתכונות הבאות המשויכות לאובייקט זה כוללים ערכים שייתכן שמשויכים כבר לאובייקט אחר בספריה המקומית.</span><span class="sxs-lookup"><span data-stu-id="1e061-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="1e061-105">אובייקט מסונכרן עם אותה כתובת proxy קיים כבר בספריה ' שירותים מקוונים של Microsoft '.</span><span class="sxs-lookup"><span data-stu-id="1e061-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="1e061-106">אין אפשרות לעדכן אובייקט זה מאחר שהתכונות הבאות המשויכות לאובייקט זה כוללים ערכים שייתכן שמשויכים כבר לאובייקט אחר בשירותי הספריה המקומיים שלך: הפקודה Username.</span><span class="sxs-lookup"><span data-stu-id="1e061-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="1e061-107">כדי לזהות ולתקן את הבעיה, להוריד ולהפעיל את [כלי תיקון שגיאות Idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="1e061-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="1e061-108">לקבלת מידע נוסף, ראה [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="1e061-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
