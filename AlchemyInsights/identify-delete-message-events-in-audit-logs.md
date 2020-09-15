---
title: זיהוי מחיקת אירועי הודעות ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696514"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="91292-102">יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו</span><span class="sxs-lookup"><span data-stu-id="91292-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="91292-103">החל מ-2019 בינואר, Microsoft מפעיל רישום של ביקורת תיבת דואר כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="91292-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="91292-104">אחרת, כדי לסקור את מחיקת אירועי הודעות עבור משתמש ספציפי, עליך להפוך את פעולות המחיקה לזמינות באופן ידני עבור ביקורת.</span><span class="sxs-lookup"><span data-stu-id="91292-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="91292-105">אם רישום ביקורת תיבת דואר כבר זמין עבור הארגון שלך או עבור המשתמש הספציפי, בצע את השלבים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="91292-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="91292-106">היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="91292-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="91292-107">לחץ על **חיפוש וחקירה** ובחר **חיפוש ביומן הביקורת**.</span><span class="sxs-lookup"><span data-stu-id="91292-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="91292-108">בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך סיום** .</span><span class="sxs-lookup"><span data-stu-id="91292-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="91292-109">ציין שם משתמש עבור המשתמש שברצונך לחקור (המשתמש שמחק את הפריטים).</span><span class="sxs-lookup"><span data-stu-id="91292-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="91292-110">בשדה **פעילויות** , בחר **הודעות שנמחקו מתוך התיקיה ' פריטים שנמחקו** ' **והעברת הודעות לתיקיה ' פריטים שנמחקו**'.</span><span class="sxs-lookup"><span data-stu-id="91292-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="91292-111">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="91292-111">Click **Search**.</span></span>

<span data-ttu-id="91292-112">בתוצאות, בחר רשומת ביקורת.</span><span class="sxs-lookup"><span data-stu-id="91292-112">In the results, select an audit record.</span></span> <span data-ttu-id="91292-113">בנשלף של הפרטים, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="91292-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="91292-114">מידע נוסף אודות הפריט שנמחק (לדוגמה, שורת הנושא ומיקום הפריט כאשר הוא נמחק) מוצג בשדה **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="91292-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="91292-115">המאפיין **ClientInfoString** יציג אם המחיקה התרחשה ב-Outlook, outlook באינטרנט (שנקרא בעבר Outlook web App), או כל מכשיר אחר.</span><span class="sxs-lookup"><span data-stu-id="91292-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="91292-116">לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="91292-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="91292-117">**הערה**: לא ניתן לאחזר פריטים שנמחקו באמצעות התכונה ' יומן ביקורת '.</span><span class="sxs-lookup"><span data-stu-id="91292-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="91292-118">כדי לאחזר הודעות שנמחקו ב-Outlook באינטרנט, ראה [שחזור פריטים שנמחקו ב-Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="91292-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
