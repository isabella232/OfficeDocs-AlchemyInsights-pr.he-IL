---
title: אירעה חריגה ממגבלת הדואר האלקטרוני היומית. זרימת העבודה מושעית.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580334"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="d5362-103">אירעה חריגה ממגבלת הדואר האלקטרוני היומית.</span><span class="sxs-lookup"><span data-stu-id="d5362-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="d5362-104">זרימת העבודה מושעית.</span><span class="sxs-lookup"><span data-stu-id="d5362-104">Workflow is suspended.</span></span>

<span data-ttu-id="d5362-105">שגיאה זו עשויה להתקבל בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d5362-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="d5362-106">ברשותך זרימת עבודה ב-SharePoint Online המשתמשת בסוג פלטפורמת זרימת העבודה sharepoint 2010 או SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d5362-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="d5362-107">תצורת זרימת העבודה מוגדרת לשליחת הודעת דואר אלקטרוני מותאמת אישית ליותר מ-200 משתמשים בכל פעם, יותר מ-10,000 נמענים ביום, או יותר מ-30 הודעות בדקה.</span><span class="sxs-lookup"><span data-stu-id="d5362-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="d5362-108">בעת הפעלת זרימת העבודה, הודעת הדואר האלקטרוני אינה נשלחת ואתה מבחין בהתנהגות הבאה:</span><span class="sxs-lookup"><span data-stu-id="d5362-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="d5362-109">עבור זרימת עבודה באמצעות סוג פלטפורמת SharePoint 2013, אתה גולש לדף ' **מצב זרימת עבודה** '.</span><span class="sxs-lookup"><span data-stu-id="d5362-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="d5362-110">בדף ' מצב זרימת עבודה ', **המצב הפנימי** מוגדר **כהתחלתי**ובבלון המידע מציג **אפשרות לשלוח לנמען**.</span><span class="sxs-lookup"><span data-stu-id="d5362-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="d5362-111">כדי לעקוף בעיה זו, הגדר את זרימת העבודה שלך לשליחת הודעות דואר אלקטרוני מבלי לחרוג [ממגבלות השולח המקוון של Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="d5362-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="d5362-112">לדוגמה, השתמש בהשהיה בזרימת העבודה, שלח את הדואר האלקטרוני לקבוצת Microsoft 365, קבוצת תפוצה או קבוצת אבטחה זמינה בדואר, או שלח את ההודעה לפחות מ-200 נמענים בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="d5362-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="d5362-113">לקבלת מידע נוסף, עיין [במאמר](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)הבא.</span><span class="sxs-lookup"><span data-stu-id="d5362-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d5362-114">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="d5362-114">Related topics</span></span>
- [<span data-ttu-id="d5362-115">צור זרימה</span><span class="sxs-lookup"><span data-stu-id="d5362-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d5362-116">SharePoint וזרימה</span><span class="sxs-lookup"><span data-stu-id="d5362-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 