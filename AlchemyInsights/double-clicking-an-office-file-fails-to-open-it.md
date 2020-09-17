---
title: לחיצה כפולה על קובץ Office אינה מצליחה לפתוח אותו
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812080"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="1bfbb-102">לחיצה כפולה על קובץ Office אינה מצליחה לפתוח אותו</span><span class="sxs-lookup"><span data-stu-id="1bfbb-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="1bfbb-103">לאחר לחיצה כפולה על קובץ Office, ייתכן שתראה את התוכנית פתוחה אך הקובץ עצמו אינו נפתח.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="1bfbb-104">לחלופין, ייתכן שתקבל את השגיאה: "אירעה בעיה בשליחת הפקודה לתוכנית".</span><span class="sxs-lookup"><span data-stu-id="1bfbb-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="1bfbb-105">יש סיבות רבות לכך, אך שני הפתרונות הנפוצים ביותר הם:</span><span class="sxs-lookup"><span data-stu-id="1bfbb-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="1bfbb-106">מתוך Excel, ודא שהאפשרות DDE אינה מסומנת.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="1bfbb-107">ניתן למצוא את האפשרות על-ידי יצירת חוברת עבודה חדשה ולאחר מכן בחירת ' **אפשרויות קובץ > ' > מתקדמות**'.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="1bfbb-108">במקטע **כללי** , בטל את הסימון **באפשרות התעלם מיישומים אחרים המשתמשים בחילופי מידע דינאמיים (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="1bfbb-109">הפעיל תיקון מקוון כדי לשחזר הגדרות ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="1bfbb-110">לחץ על לחצן ' התחל ' של Windows וחפש את "לוח הבקרה".</span><span class="sxs-lookup"><span data-stu-id="1bfbb-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="1bfbb-111">פתח את **לוח הבקרה**ועבור אל **תוכניות _GT_ תוכניות ותכונות**.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="1bfbb-112">לאחר מכן לחץ באמצעות לחצן העכבר הימני על **Microsoft Office [Version]** **ובחר שינוי תיקון מקוון של >**.</span><span class="sxs-lookup"><span data-stu-id="1bfbb-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="1bfbb-113">אם אף אחד מפתרונות אלה אינו פועל, ניתן למצוא רשימה מלאה יותר של פתרונות במאמר התמיכה, [לחיצה כפולה על קובץ Office אינה מצליחה לפתוח אותו](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="1bfbb-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
