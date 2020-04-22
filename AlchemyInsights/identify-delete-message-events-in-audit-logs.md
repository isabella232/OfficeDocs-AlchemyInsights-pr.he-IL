---
title: זיהוי אירועי הודעות מחיקה ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716497"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="5c64c-102">יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו</span><span class="sxs-lookup"><span data-stu-id="5c64c-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="5c64c-103">החל מינואר 2019, Microsoft מופעלת כברירת מחדל ברישום ביקורת תיבת דואר.</span><span class="sxs-lookup"><span data-stu-id="5c64c-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="5c64c-104">אחרת, כדי לסקור אירועי הודעה עבור משתמש מסוים, עליך להפוך באופן ידני את פעולות המחיקה לביקורת.</span><span class="sxs-lookup"><span data-stu-id="5c64c-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="5c64c-105">אם רישום ביקורת תיבת דואר זמין כבר עבור הארגון שלך או עבור המשתמש הספציפי, בצע את השלבים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="5c64c-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="5c64c-106">היכנס ל- [Microsoft 365 האבטחה _ Ampp_e מרכז התאימות](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="5c64c-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="5c64c-107">לחץ על **חיפוש וחקירה** ובחר **חיפוש יומן רישום ביקורת**.</span><span class="sxs-lookup"><span data-stu-id="5c64c-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="5c64c-108">בחר את טווח התאריכים **בתאריך ההתחלה** ושדות **הסיום** .</span><span class="sxs-lookup"><span data-stu-id="5c64c-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="5c64c-109">ציין שם משתמש עבור המשתמש שברצונך לחקור (המשתמש שמחק את הפריטים).</span><span class="sxs-lookup"><span data-stu-id="5c64c-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="5c64c-110">בשדה ' **פעילויות** ', בחר **הודעות שנמחקו מהתיקיה ' פריטים שנמחקו** ' והעברת **הודעות לפריטים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="5c64c-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="5c64c-111">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="5c64c-111">Click **Search**.</span></span>

<span data-ttu-id="5c64c-112">בתוצאות, בחר ברשומת ביקורת.</span><span class="sxs-lookup"><span data-stu-id="5c64c-112">In the results, select an audit record.</span></span> <span data-ttu-id="5c64c-113">בתפריט הפרטי, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="5c64c-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="5c64c-114">מידע נוסף אודות הפריט שנמחק (לדוגמה, שורת הנושא ומיקום הפריט בעת המחיקה) מוצג בשדה ' **הקצאת** המים '.</span><span class="sxs-lookup"><span data-stu-id="5c64c-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="5c64c-115">המאפיין **מחרוזת לקוחוה** יציג אם המחיקה התרחשה ב-Outlook, outlook באינטרנט (הידוע בעבר כ-Outlook web App), או כל התקן אחר.</span><span class="sxs-lookup"><span data-stu-id="5c64c-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="5c64c-116">לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="5c64c-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="5c64c-117">**הערה**: לא ניתן לאחזר פריטים שנמחקו באמצעות תכונת יומן הביקורת.</span><span class="sxs-lookup"><span data-stu-id="5c64c-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="5c64c-118">כדי לאחזר הודעות שנמחקו ב-Outlook באינטרנט, ראה [שחזור פריטים שנמחקו ב-Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="5c64c-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
