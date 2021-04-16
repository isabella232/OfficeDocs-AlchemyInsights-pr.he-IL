---
title: לחיצה כפולה על קובץ Office נכשלת בפתיחה שלו
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814806"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="e8aa9-102">לחיצה כפולה על קובץ Office נכשלת בפתיחה שלו</span><span class="sxs-lookup"><span data-stu-id="e8aa9-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="e8aa9-103">לאחר לחיצה כפולה על קובץ Office, ייתכן שהתוכנית תיפתח, אך הקובץ עצמו אינו נפתח.</span><span class="sxs-lookup"><span data-stu-id="e8aa9-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="e8aa9-104">לחלופין, ייתכן שאתה מקבל את השגיאה: "אירעה בעיה בשליחת הפקודה לתוכנית".</span><span class="sxs-lookup"><span data-stu-id="e8aa9-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="e8aa9-105">קיימים סיבות רבות לכך, אך שני הפתרונות הנפוצים ביותר הם:</span><span class="sxs-lookup"><span data-stu-id="e8aa9-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="e8aa9-106">מתוך Excel, ודא שהאפשרות DDE אינה מסומנת.</span><span class="sxs-lookup"><span data-stu-id="e8aa9-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="e8aa9-107">ניתן למצוא את האפשרות על-ידי יצירת חוברת עבודה חדשה ולאחר מכן בחירת **קובץ > אפשרויות > מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="e8aa9-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="e8aa9-108">במקטע **כללי,** בטל את הסימון של התעלם **מיישומים אחרים המשתמשים בחילופי נתונים דינאמיים (DDE).**</span><span class="sxs-lookup"><span data-stu-id="e8aa9-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="e8aa9-109">הפעל תיקון מקוון כדי לשחזר הגדרות ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="e8aa9-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="e8aa9-110">לחץ על לחצן התחל של Windows וחפש את "לוח הבקרה".</span><span class="sxs-lookup"><span data-stu-id="e8aa9-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="e8aa9-111">פתח את **לוח הבקרה,** עבור אל **תוכניות > תוכניות ותכונות**.</span><span class="sxs-lookup"><span data-stu-id="e8aa9-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="e8aa9-112">לאחר מכן לחץ באמצעות לחצן **העכבר הימני על Microsoft Office [גירסה]** ובחר שנה > **תיקון מקוון**.</span><span class="sxs-lookup"><span data-stu-id="e8aa9-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="e8aa9-113">אם אף אחד מפתרונות אלה אינו פועל, ניתן למצוא רשימה מלאה יותר של פתרונות במאמר התמיכה, לחיצה כפולה [על קובץ Office אינה מצליחה לפתוח אותו.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="e8aa9-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
