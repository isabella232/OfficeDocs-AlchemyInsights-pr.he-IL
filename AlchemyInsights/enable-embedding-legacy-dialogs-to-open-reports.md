---
title: הפיכת הטבעה של תיבות דו-שיח מדור קודם לזמינה כדי לפתוח דוחות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814265"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="c067c-102">הפיכת הטבעה של תיבות דו-שיח מדור קודם לזמינה כדי לפתוח דוחות</span><span class="sxs-lookup"><span data-stu-id="c067c-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="c067c-103">**מאפיין הבעיה**</span><span class="sxs-lookup"><span data-stu-id="c067c-103">**Symptom**</span></span>

<span data-ttu-id="c067c-104">למשתמשים אין אפשרות לפתוח דוחות.</span><span class="sxs-lookup"><span data-stu-id="c067c-104">Users are unable to open reports.</span></span> <span data-ttu-id="c067c-105">"משהו השתבש.</span><span class="sxs-lookup"><span data-stu-id="c067c-105">"Something has gone wrong.</span></span> <span data-ttu-id="c067c-106">עיין בפרטים הטכניים לקבלת פרטים נוספים."</span><span class="sxs-lookup"><span data-stu-id="c067c-106">Check technical details for more details."</span></span>

<span data-ttu-id="c067c-107">**סיבה**</span><span class="sxs-lookup"><span data-stu-id="c067c-107">**Cause**</span></span>

<span data-ttu-id="c067c-108">הדוחות נכשלים בטעינה ב- UCI עם השגיאה "Form מתאר הוא Null או לא מוגדר".</span><span class="sxs-lookup"><span data-stu-id="c067c-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="c067c-109">דוחות ב- UCI עדיין דורשים תיבות דו-שיח מדור קודם, כך שמערכת הלקוח צריכה לאפשר שימוש ב- *allowlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="c067c-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="c067c-110">**פתרון**</span><span class="sxs-lookup"><span data-stu-id="c067c-110">**Solution**</span></span>

1. <span data-ttu-id="c067c-111">עבור אל **הגדרות >ניהול > הגדרות > כללי**.</span><span class="sxs-lookup"><span data-stu-id="c067c-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="c067c-112">הגדר "אפשר הטבעה של תיבות דו-שיח מדור קודם מסוימות בלקוח דפדפן Unified Interface" **ל'כן'.**</span><span class="sxs-lookup"><span data-stu-id="c067c-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
