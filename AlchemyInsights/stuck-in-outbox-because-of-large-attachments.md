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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232631"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="f485e-102">תיקון הודעות התקועות בתיבת הדואר היוצא</span><span class="sxs-lookup"><span data-stu-id="f485e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="f485e-103">אנו ממליצים שתתחיל בהפעלת התרחיש ["אני נתקל בבעיות בשליחה, קבלה או חיפוש של הודעות דואר אלקטרוני"](https://aka.ms/SaRA-OutlookSendReceive) מתוך כלי [מסייע התמיכה והשחזור של Microsoft](https://diagnostics.office.com/#/) במחשב המושפע.</span><span class="sxs-lookup"><span data-stu-id="f485e-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="f485e-104">כאשר הודעה נתקעת בתיבת הדואר היוצא שלך, הסיבה הסבירה ביותר היא קובץ מצורף גדול או האפשרות "שלח מיד כאשר מחובר" אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="f485e-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="f485e-105">**הסר את הקובץ המצורף הגדול**</span><span class="sxs-lookup"><span data-stu-id="f485e-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="f485e-106">לחץ על **שליחה/קבלה** > של**עבודה במצב לא מקוון**.</span><span class="sxs-lookup"><span data-stu-id="f485e-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="f485e-107">בחלונית הניווט, לחץ על **תיבת דואר יוצא**.</span><span class="sxs-lookup"><span data-stu-id="f485e-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="f485e-108">מכאן, אתה יכול:</span><span class="sxs-lookup"><span data-stu-id="f485e-108">From here, you can:</span></span> 
    - <span data-ttu-id="f485e-109">מחק את ההודעה.</span><span class="sxs-lookup"><span data-stu-id="f485e-109">Delete the message.</span></span> <span data-ttu-id="f485e-110">פשוט בחר אותו ולחץ על **Delete**.</span><span class="sxs-lookup"><span data-stu-id="f485e-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="f485e-111">גרור את ההודעה **לתיקיית הטיוטות**, לחץ פעמיים כדי לפתוח את ההודעה ומחק את הקובץ המצורף (לחץ עליו ולחץ על **delete**).</span><span class="sxs-lookup"><span data-stu-id="f485e-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="f485e-112">אם שגיאה מציינת ש-Outlook מנסה לשדר את ההודעה, סגור את Outlook.</span><span class="sxs-lookup"><span data-stu-id="f485e-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="f485e-113">ייתכן שייקח כמה דקות. לצאת מכאן</span><span class="sxs-lookup"><span data-stu-id="f485e-113">It may take a few moments to exit.</span></span> <span data-ttu-id="f485e-114">אם Outlook אינו סגור, הקש **Ctrl + Alt + Delete** ולחץ על **הפעל את מנהל המשימות**.</span><span class="sxs-lookup"><span data-stu-id="f485e-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="f485e-115">במנהל המשימות, בחר בכרטיסיה **תהליכים** , גלול למטה ל-outlook. exe ולחץ על **סיום תהליך**.</span><span class="sxs-lookup"><span data-stu-id="f485e-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="f485e-116">לאחר הסגירה של Outlook, הפעל מחדש את Outlook וחזור על שלבים 2-3.</span><span class="sxs-lookup"><span data-stu-id="f485e-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="f485e-117">לאחר הסרת הקובץ המצורף, לחץ על **שלח/קבל** > **עבודה במצב לא מקוון** כדי לבטל את הבחירה בלחצן ולחדש את העבודה באופן מקוון.</span><span class="sxs-lookup"><span data-stu-id="f485e-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="f485e-118">הודעות מקבל גם נתקע בתיבת הדואר היוצא בעת לחיצה על **שלח**, אך אינך מחובר.</span><span class="sxs-lookup"><span data-stu-id="f485e-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="f485e-119">לחץ על **שלח/קבל** והסתכל בלחצן **עבודה לא מקוון** .</span><span class="sxs-lookup"><span data-stu-id="f485e-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="f485e-120">. אם זה כחול, אתה מנותק</span><span class="sxs-lookup"><span data-stu-id="f485e-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="f485e-121">לחץ עליו כדי להתחבר (הלחצן הופך לבן) ולחץ על **שלח הכל**.</span><span class="sxs-lookup"><span data-stu-id="f485e-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="f485e-122">**אפשר שליחה מיידית בעת ההתחברות**</span><span class="sxs-lookup"><span data-stu-id="f485e-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="f485e-123">בכרטיסיה קובץ, לחץ על **אפשרויות**.</span><span class="sxs-lookup"><span data-stu-id="f485e-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="f485e-124">בתיבת הדו אפשרויות Outlook, לחץ על **מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="f485e-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="f485e-125">במקטע שלח וקבל, לחץ כדי לאפשר **שליחה באופן מיידי בעת ההתחברות**.</span><span class="sxs-lookup"><span data-stu-id="f485e-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="f485e-126">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="f485e-126">Click **OK**.</span></span>
 
<span data-ttu-id="f485e-127">לפרטים מלאים, ראו:</span><span class="sxs-lookup"><span data-stu-id="f485e-127">For full details, see:</span></span>
- [<span data-ttu-id="f485e-128">וידאו: שלח או מחק דוא ל תקוע</span><span class="sxs-lookup"><span data-stu-id="f485e-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="f485e-129">דואר אלקטרוני נשאר בתיקיה ' תיבת דואר יוצא ' עד שתיזום באופן ידני פעולת שליחה/קבלה ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="f485e-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
