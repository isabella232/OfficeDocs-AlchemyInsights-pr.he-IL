---
title: הפעלת 'אבחון זיכרון של Windows' ב- Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826668"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="5ed39-102">הפעלת 'אבחון זיכרון של Windows' ב- Windows 10</span><span class="sxs-lookup"><span data-stu-id="5ed39-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="5ed39-103">אם Windows ואפליקציות במחשב קורסים, קופאים או פועלים באופן לא יציב, ייתכן שיש לך בעיה בזיכרון המחשב (RAM).</span><span class="sxs-lookup"><span data-stu-id="5ed39-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="5ed39-104">באפשרותך להפעיל את אבחון הזיכרון של Windows כדי לבדוק אם יתו בעיות בזיכרון ה- RAM של המחשב.</span><span class="sxs-lookup"><span data-stu-id="5ed39-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="5ed39-105">בתיבת החיפוש בשורת המשימות, הקלד אבחון **זיכרון** ולאחר מכן בחר אבחון **זיכרון של Windows**.</span><span class="sxs-lookup"><span data-stu-id="5ed39-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="5ed39-106">כדי להפעיל את האבחון, המחשב צריך להפעיל מחדש.</span><span class="sxs-lookup"><span data-stu-id="5ed39-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="5ed39-107">יש לך אפשרות להפעיל מחדש באופן מיידי (שמור את עבודתך וסגור תחילה מסמכים והודעות דואר אלקטרוני פתוחים), או תזמן את האבחון לפעול באופן אוטומטי בפעם הבאה שהמחשב יופעל מחדש:</span><span class="sxs-lookup"><span data-stu-id="5ed39-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![אבחון זיכרון של Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="5ed39-109">כאשר המחשב יופעל מחדש, כלי **אבחון הזיכרון של Windows יופעל** באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="5ed39-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="5ed39-110">המצב וההתקדמות יוצגו בעת הפעלת האבחון, ויש לך אפשרות לבטל את האבחון על-ידי לחיצה על **מקש ESC** בלוח המקשים.</span><span class="sxs-lookup"><span data-stu-id="5ed39-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="5ed39-111">לאחר השלמת האבחון, Windows יתחיל כרגיל.</span><span class="sxs-lookup"><span data-stu-id="5ed39-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="5ed39-112">מיד לאחר ההפעלה מחדש, כאשר שולחן העבודה מופיע, תופיע הודעה (לצד סמל **מרכז** הפעולות בשורת המשימות), כדי לציין אם נמצאו שגיאות זיכרון כלשהן.</span><span class="sxs-lookup"><span data-stu-id="5ed39-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="5ed39-113">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="5ed39-113">For example:</span></span>

<span data-ttu-id="5ed39-114">הנה סמל מרכז הפעולות:</span><span class="sxs-lookup"><span data-stu-id="5ed39-114">Here's the Action Center icon:</span></span> ![סמל מרכז הפעולות](media/action-center-icon.png) 

<span data-ttu-id="5ed39-116">והודעה לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="5ed39-116">And a sample notification:</span></span> ![אין שגיאות זיכרון](media/no-memory-errors.png)

<span data-ttu-id="5ed39-118">אם החמצת את ההודעה, באפשרותך לבחור בסמל **מרכז** הפעולות בשורת המשימות כדי להציג את **מרכז** הפעולות ולראות רשימה ניתנת לגלילה של הודעות.</span><span class="sxs-lookup"><span data-stu-id="5ed39-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="5ed39-119">כדי לסקור מידע מפורט, **הקלד אירוע** בתיבת החיפוש בשורת המשימות ולאחר מכן בחר **מציג האירועים**.</span><span class="sxs-lookup"><span data-stu-id="5ed39-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="5ed39-120">בחלונית **הימנית** של מציג האירועים, נווט אל **יומני הרישום של Windows > מערכת**.</span><span class="sxs-lookup"><span data-stu-id="5ed39-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="5ed39-121">בחלונית השמאלית, סרוק את הרשימה בעת  התסת עמודה, עד שאתה רואה אירועים עם ערך מקור **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="5ed39-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="5ed39-122">סמן כל אירוע כזה ו תראה את פרטי התוצאה בתיבה תחת **הכרטיסיה כללי** מתחת לרשימה.</span><span class="sxs-lookup"><span data-stu-id="5ed39-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
