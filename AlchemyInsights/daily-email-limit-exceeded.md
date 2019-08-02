---
title: חריגה ממגבלת דואר אלקטרוני יומי. זרימת עבודה מושעית.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059640"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="d955b-103">חריגה ממגבלת דואר אלקטרוני יומי.</span><span class="sxs-lookup"><span data-stu-id="d955b-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="d955b-104">זרימת עבודה מושעית.</span><span class="sxs-lookup"><span data-stu-id="d955b-104">Workflow is suspended.</span></span>

<span data-ttu-id="d955b-105">שגיאה זו עשויה להתקבל בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d955b-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="d955b-106">יש לך זרימת עבודה ב- SharePoint במצב מקוון שבו הוא משתמש SharePoint 2010 או סוג פלטפורמה זרימת עבודה של SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d955b-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="d955b-107">זרימת העבודה נקבעה כדי לשלוח הודעת דואר אלקטרוני מותאמות אישית משתמשים יותר מ- 200 בכל פעם, למעלה מ- 10,000 נמענים בכל יום או יותר מ- 30 הודעות לדקה.</span><span class="sxs-lookup"><span data-stu-id="d955b-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="d955b-108">כאשר אתה מפעיל את זרימת העבודה, ההודעה לא תישלח ולאחר תבחין בהתנהגות הבאה:</span><span class="sxs-lookup"><span data-stu-id="d955b-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="d955b-109">עבור זרימת עבודה באמצעות סוג פלטפורמת SharePoint 2013, דפדף אל דף **מצב זרימת העבודה** .</span><span class="sxs-lookup"><span data-stu-id="d955b-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="d955b-110">בדף ' מצב זרימת עבודה ', **מצב פנימי** מוגדר **הופעל**, ומציג בלון המידע **אין אפשרות לשלוח לנמען**.</span><span class="sxs-lookup"><span data-stu-id="d955b-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="d955b-111">כדי לעקוף בעיה זו, קביעת התצורה של זרימת העבודה שלך כדי לשלוח הודעות דואר אלקטרוני מבלי לחרוג [ממגבלות השולח Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="d955b-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="d955b-112">לדוגמה, השתמש השהיה בזרימת העבודה, הדואר האלקטרוני לקבוצה Office 365, קבוצת תפוצה או קבוצת אבטחה דואר זמין או לשלוח את ההודעה לנמענים פחות מ- 200 בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="d955b-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="d955b-113">לקבלת מידע נוסף, עיין [במאמר](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)הבא.</span><span class="sxs-lookup"><span data-stu-id="d955b-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d955b-114">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="d955b-114">Related topics</span></span>
- [<span data-ttu-id="d955b-115">צור זרימה</span><span class="sxs-lookup"><span data-stu-id="d955b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d955b-116">SharePoint וזרימה</span><span class="sxs-lookup"><span data-stu-id="d955b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 