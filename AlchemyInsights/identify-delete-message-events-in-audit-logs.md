---
title: לזהות אירועים ההודעה מחק יומני ביקורת
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416711"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="14e2e-102">יומני ביקורת עבור הודעות דואר אלקטרוני שנמחקו</span><span class="sxs-lookup"><span data-stu-id="14e2e-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="14e2e-103">החל ב- 2019 בינואר, הוא הפעלת Microsoft ביקורת תיבות דואר רישום כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="14e2e-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="14e2e-104">אחרת, כדי לסקור את אירועי הודעת מחיקה עבור משתמש מסוים, עליך לאפשר באופן ידני את פעולות מחיקה לביקורת.</span><span class="sxs-lookup"><span data-stu-id="14e2e-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="14e2e-105">אם תיבת הדואר ביקורת רישום כבר זמין עבור הארגון שלך או עבור משתמש מסוים, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="14e2e-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="14e2e-106">היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="14e2e-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="14e2e-107">לחץ על **חיפוש ויצירת החקירה** ובחר באפשרות **החיפוש יומן ביקורת**.</span><span class="sxs-lookup"><span data-stu-id="14e2e-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="14e2e-108">בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** .</span><span class="sxs-lookup"><span data-stu-id="14e2e-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="14e2e-109">ציין את שם המשתמש עבור המשתמש שברצונך לבדוק (המשתמש על הפריטים שנמחקו).</span><span class="sxs-lookup"><span data-stu-id="14e2e-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="14e2e-110">בשדה ' **פעילויות** ', בחר **הודעות שנמחקו מהתיקיה פריטים שנמחקו** והודעות **Moved לתיקיה פריטים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="14e2e-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="14e2e-111">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="14e2e-111">Click **Search**.</span></span>

<span data-ttu-id="14e2e-112">בתוצאות, בחר את רשומת הביקורת.</span><span class="sxs-lookup"><span data-stu-id="14e2e-112">In the results, select an audit record.</span></span> <span data-ttu-id="14e2e-113">תפריט נשלף של פרטים, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="14e2e-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="14e2e-114">מידע נוסף אודות הפריט שנמחק (לדוגמה, את שורת הנושא ואת המיקום של הפריט בעת שהוא נמחק) מוצג בשדה **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="14e2e-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="14e2e-115">המאפיין **ClientInfoString** יציג אם המחיקה אירעה ב- Outlook, Outlook באינטרנט (שכונתה בעבר Outlook Web App), או כל התקן אחר.</span><span class="sxs-lookup"><span data-stu-id="14e2e-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="14e2e-116">לקבלת מידע נוסף, ראה [קביעת שהגדיר העברה עבור תיבת דואר אלקטרוני](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="14e2e-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="14e2e-117">**הערה**: אין אפשרות לאחזר פריטים שנמחקו באמצעות התכונה ביומן הביקורת.</span><span class="sxs-lookup"><span data-stu-id="14e2e-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="14e2e-118">כדי לאחזר הודעות שנמחקו ב- Outlook באינטרנט, ראה [שחזור פריטים ב- Outlook Web App שנמחקו](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="14e2e-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
