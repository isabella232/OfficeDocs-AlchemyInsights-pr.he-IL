---
title: חריגה ממגבלת דואר אלקטרוני יומית. זרימת העבודה מושעית.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731564"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="4daa5-103">חריגה ממגבלת דואר אלקטרוני יומית.</span><span class="sxs-lookup"><span data-stu-id="4daa5-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="4daa5-104">זרימת העבודה מושעית.</span><span class="sxs-lookup"><span data-stu-id="4daa5-104">Workflow is suspended.</span></span>

<span data-ttu-id="4daa5-105">שגיאה זו עשויה להתקבל בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="4daa5-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="4daa5-106">יש לך זרימת עבודה ב-SharePoint Online המשתמשת בסוג פלטפורמת זרימת העבודה של SharePoint 2010 או SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="4daa5-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="4daa5-107">זרימת העבודה מוגדרת לשליחת הודעת דואר אלקטרוני מותאמת אישית ליותר מ-200 משתמשים בכל פעם, יותר מ-10,000 נמענים לכל יום, או יותר מ-30 הודעות בדקה.</span><span class="sxs-lookup"><span data-stu-id="4daa5-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="4daa5-108">כאשר תפעיל את זרימת העבודה, הודעת הדואר האלקטרוני לא תישלח ותשים לב לאופן הפעולה הבא:</span><span class="sxs-lookup"><span data-stu-id="4daa5-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="4daa5-109">עבור זרימת עבודה באמצעות סוג הפלטפורמה של SharePoint 2013, עליך לדפדף לדף ' **מצב זרימת עבודה** '.</span><span class="sxs-lookup"><span data-stu-id="4daa5-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="4daa5-110">בדף ' מצב זרימת עבודה ', **המצב הפנימי** מוגדר **להתחיל**, ובלון המידע אינו מציג **אפשרות לשלוח לנמען**.</span><span class="sxs-lookup"><span data-stu-id="4daa5-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="4daa5-111">כדי לעקוף בעיה זו, קבע את התצורה של זרימת העבודה לשליחת הודעות דואר אלקטרוני מבלי לחרוג [ממגבלות השולח של Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="4daa5-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="4daa5-112">לדוגמה, השתמש בהשהיה בזרימת העבודה, שלח את הדואר האלקטרוני לקבוצה של Microsoft 365, קבוצת תפוצה או קבוצת אבטחה המותאמת לשימוש בדואר, או שלח את ההודעה לפחות מ-200 נמענים בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="4daa5-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="4daa5-113">לקבלת מידע נוסף, עיין [במאמר](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)הבא.</span><span class="sxs-lookup"><span data-stu-id="4daa5-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="4daa5-114">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="4daa5-114">Related topics</span></span>
- [<span data-ttu-id="4daa5-115">יצירת זרימה</span><span class="sxs-lookup"><span data-stu-id="4daa5-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="4daa5-116">SharePoint ו-Flow</span><span class="sxs-lookup"><span data-stu-id="4daa5-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 