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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241253"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="f36a1-102">תיקון הודעות התקועות בתיבת הדואר היוצא</span><span class="sxs-lookup"><span data-stu-id="f36a1-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="f36a1-103">אנו ממליצים שתתחיל בהפעלת התרחיש ["אני נתקל בבעיות בשליחה, קבלה או חיפוש של הודעות דואר אלקטרוני"](https://aka.ms/SaRA-OutlookSendReceive) מתוך הכלי [של מסייע התמיכה והשחזור של Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="f36a1-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="f36a1-104">כאשר הודעה נתקעת בתיבת הדואר היוצא שלך, הסיבה הסבירה ביותר היא קובץ מצורף גדול או האפשרות "שלח מיד כאשר מחובר" אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="f36a1-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="f36a1-105">**הסר את הקובץ המצורף הגדול**</span><span class="sxs-lookup"><span data-stu-id="f36a1-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="f36a1-106">ב-Outlook, בחר באפשרות **שלח/קבל** > **עבודה במצב לא מקוון**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="f36a1-107">בחלונית הניווט, בחר **תיבת דואר יוצא**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="f36a1-108">מכאן, אתה יכול:</span><span class="sxs-lookup"><span data-stu-id="f36a1-108">From here, you can:</span></span> 
    - <span data-ttu-id="f36a1-109">מחק את ההודעה (בחר אותה ולאחר מכן בחר **במחק**).</span><span class="sxs-lookup"><span data-stu-id="f36a1-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="f36a1-110">גרור את ההודעה לתיקיה טיוטות, לחץ פעמיים כדי לפתוח אותה והסר את הקובץ המצורף בחר בו ולאחר מכן בחר **במחק**).</span><span class="sxs-lookup"><span data-stu-id="f36a1-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="f36a1-111">אם מתקבלת שגיאה המציינת ש-Outlook מנסה לשדר את ההודעה, סגור את Outlook.</span><span class="sxs-lookup"><span data-stu-id="f36a1-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="f36a1-112">ייתכן שייקח כמה דקות. לצאת מכאן</span><span class="sxs-lookup"><span data-stu-id="f36a1-112">It may take a few moments to exit.</span></span> <span data-ttu-id="f36a1-113">אם Outlook אינו סגור, הקש Ctrl + Alt + Delete ובחר באפשרות ' **הפעל מנהל המשימות**'.</span><span class="sxs-lookup"><span data-stu-id="f36a1-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="f36a1-114">במנהל המשימות, בחר בכרטיסיה **תהליכים** , גלול למטה ל-outlook. exe ובחר **בסוף תהליך**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="f36a1-115">לאחר הסגירה של Outlook, הפעל אותו מחדש וחזור על שלבים 2 ו-3.</span><span class="sxs-lookup"><span data-stu-id="f36a1-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="f36a1-116">לאחר הסרת הקובץ המצורף, לחץ על **שלח/קבל** > **עבודה במצב לא מקוון** כדי לחדש את העבודה באופן מקוון.</span><span class="sxs-lookup"><span data-stu-id="f36a1-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="f36a1-117">הודעות מקבל גם נתקע בתיבת הדואר היוצא בעת לחיצה על **שלח**, אך אינך מחובר.</span><span class="sxs-lookup"><span data-stu-id="f36a1-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="f36a1-118">לחץ על **שלח/קבל** והסתכל בלחצן **עבודה לא מקוון** .</span><span class="sxs-lookup"><span data-stu-id="f36a1-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="f36a1-119">. אם זה כחול, אתה מנותק</span><span class="sxs-lookup"><span data-stu-id="f36a1-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="f36a1-120">לחץ עליו כדי להתחבר (הלחצן הופך לבן) ולחץ על **שלח הכל**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="f36a1-121">**אפשר שליחה מיידית בעת ההתחברות**</span><span class="sxs-lookup"><span data-stu-id="f36a1-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="f36a1-122">בכרטיסיה קובץ, לחץ על **אפשרויות**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="f36a1-123">בתיבת הדו אפשרויות Outlook, לחץ על **מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="f36a1-124">במקטע שלח וקבל, לחץ כדי לאפשר **שליחה באופן מיידי בעת ההתחברות**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="f36a1-125">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="f36a1-125">Click **OK**.</span></span>
 
<span data-ttu-id="f36a1-126">לפרטים מלאים, ראו:</span><span class="sxs-lookup"><span data-stu-id="f36a1-126">For full details, see:</span></span>
- [<span data-ttu-id="f36a1-127">וידאו: שלח או מחק דוא ל תקוע</span><span class="sxs-lookup"><span data-stu-id="f36a1-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="f36a1-128">דואר אלקטרוני נשאר בתיקיה ' תיבת דואר יוצא ' עד שתיזום באופן ידני פעולת שליחה/קבלה ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="f36a1-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
