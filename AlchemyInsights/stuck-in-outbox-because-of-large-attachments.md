---
title: תקוע בתיבת דואר יוצא בגלל קבצים מצורפים גדולים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441307"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="3e616-102">תיקון הודעות התקועות בתיבת הדואר היוצא</span><span class="sxs-lookup"><span data-stu-id="3e616-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="3e616-103">אנו ממליצים שתתחיל בהפעלת התרחיש ["אני נתקל בבעיות בשליחה, קבלה או חיפוש של הודעות דואר אלקטרוני"](https://aka.ms/SaRA-OutlookSendReceive) מתוך הכלי [של מסייע התמיכה והשחזור של Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="3e616-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="3e616-104">כאשר הודעה נתקעת בתיבת הדואר היוצא, הסיבות הסבירות ביותר הן:</span><span class="sxs-lookup"><span data-stu-id="3e616-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="3e616-105">. החזקות גדולות</span><span class="sxs-lookup"><span data-stu-id="3e616-105">Large attachments.</span></span>
- <span data-ttu-id="3e616-106">האפשרות **שלח מיד בעת ההתחברות** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="3e616-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="3e616-107">כדי להסיר קבצים מצורפים גדולים:</span><span class="sxs-lookup"><span data-stu-id="3e616-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="3e616-108">ב-Outlook, בחר באפשרות **שלח/קבל** > **עבודה במצב לא מקוון**.</span><span class="sxs-lookup"><span data-stu-id="3e616-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="3e616-109">בחלונית הניווט, בחר **תיבת דואר יוצא**.</span><span class="sxs-lookup"><span data-stu-id="3e616-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="3e616-110">מכאן, אתה יכול:</span><span class="sxs-lookup"><span data-stu-id="3e616-110">From here, you can:</span></span> 
    - <span data-ttu-id="3e616-111">מחק את ההודעה (בחר אותה ולאחר מכן בחר **במחק**).</span><span class="sxs-lookup"><span data-stu-id="3e616-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="3e616-112">גרור את ההודעה לתיקיה טיוטות, לחץ פעמיים כדי לפתוח אותה והסר את הקובץ המצורף בחר בו ולאחר מכן בחר **במחק**).</span><span class="sxs-lookup"><span data-stu-id="3e616-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="3e616-113">אם מתקבלת שגיאה המציינת ש-Outlook מנסה לשדר את ההודעה, סגור את Outlook.</span><span class="sxs-lookup"><span data-stu-id="3e616-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="3e616-114">ייתכן שייקח כמה דקות. לצאת מכאן</span><span class="sxs-lookup"><span data-stu-id="3e616-114">It may take a few moments to exit.</span></span> <span data-ttu-id="3e616-115">אם Outlook אינו סגור, הקש Ctrl + Alt + Delete ובחר באפשרות ' **הפעל מנהל המשימות**'.</span><span class="sxs-lookup"><span data-stu-id="3e616-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="3e616-116">במנהל המשימות, בחר בכרטיסיה **תהליכים** , גלול למטה ל-outlook. exe ובחר **בסוף תהליך**.</span><span class="sxs-lookup"><span data-stu-id="3e616-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="3e616-117">לאחר הסגירה של Outlook, הפעל אותו מחדש וחזור על שלבים 2 ו-3.</span><span class="sxs-lookup"><span data-stu-id="3e616-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="3e616-118">לאחר הסרת הקובץ המצורף, לחץ על **שלח/קבל** > **עבודה במצב לא מקוון** כדי לחדש את העבודה באופן מקוון.</span><span class="sxs-lookup"><span data-stu-id="3e616-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="3e616-119">הודעות מקבל גם נתקע בתיבת הדואר היוצא בעת לחיצה על **שלח**, אך אינך מחובר.</span><span class="sxs-lookup"><span data-stu-id="3e616-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="3e616-120">לחץ על **שלח/קבל** והסתכל בלחצן **עבודה לא מקוון** .</span><span class="sxs-lookup"><span data-stu-id="3e616-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="3e616-121">. אם זה כחול, אתה מנותק</span><span class="sxs-lookup"><span data-stu-id="3e616-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="3e616-122">בחר אותו כדי להתחבר (הלחצן הופך לבן) ולחץ על **שלח הכל**.</span><span class="sxs-lookup"><span data-stu-id="3e616-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="3e616-123">כדי להפוך את השליחה לזמינה באופן **מיידי בעת ההתחברות**:</span><span class="sxs-lookup"><span data-stu-id="3e616-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="3e616-124">בחר \*\*\*\* > \*\*\*\* אפשרויות >  קובץ**מתקדמות**.</span><span class="sxs-lookup"><span data-stu-id="3e616-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="3e616-125">במקטע **שליחה וקבלה** , בחר **בשלח מיד בעת ההתחברות**ולאחר מכן בחר **באפשרות אישור**.</span><span class="sxs-lookup"><span data-stu-id="3e616-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="3e616-126">לפרטים המלאים ראו:</span><span class="sxs-lookup"><span data-stu-id="3e616-126">For full details see:</span></span>
- [<span data-ttu-id="3e616-127">וידאו: שלח או מחק דוא ל תקוע</span><span class="sxs-lookup"><span data-stu-id="3e616-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="3e616-128">דואר אלקטרוני נשאר בתיקיה ' תיבת דואר יוצא ' עד שתיזום באופן ידני פעולת שליחה/קבלה ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="3e616-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
