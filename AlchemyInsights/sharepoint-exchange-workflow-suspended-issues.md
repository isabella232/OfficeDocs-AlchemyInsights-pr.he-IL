---
title: תחילת העבודה עם SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: a44b2c7b26895e09c24df772f1ada9a2e3483747
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735984"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="40f69-102">זרימות עבודה ב- SharePoint</span><span class="sxs-lookup"><span data-stu-id="40f69-102">Workflows in SharePoint</span></span>

<span data-ttu-id="40f69-103">אם זרימות עבודה של SharePoint לא שולח הודעות דואר אלקטרוני, הארגון שלך נתקל מגבלות השולח Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="40f69-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="40f69-104">הודעת השגיאה 'זרימת עבודה מושעית' עלולה להתרחש אם יש לך אחד מהפריטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="40f69-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="40f69-105">יש לך זרימת עבודה ב- SharePoint במצב מקוון שבו הוא משתמש SharePoint 2010 או סוג פלטפורמה זרימת עבודה של SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="40f69-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="40f69-106">זרימת העבודה נקבעה כדי לשלוח הודעת דואר אלקטרוני מותאמות אישית משתמשים יותר מ- 200 בכל פעם, למעלה מ- 10,000 נמענים בכל יום או יותר מ- 30 הודעות לדקה.</span><span class="sxs-lookup"><span data-stu-id="40f69-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="40f69-107">כאשר אתה מפעיל את זרימת העבודה, לא תישלח הודעת דואר אלקטרוני, אתה מבחין את הודעת השגיאה, מצב פנימי מוגדר מוצג מושעה או אין אפשרות לשלוח לנמען.</span><span class="sxs-lookup"><span data-stu-id="40f69-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="40f69-108">לקבלת מידע נוסף, עיין [במאמר](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)הבא.</span><span class="sxs-lookup"><span data-stu-id="40f69-108">For more information, please refer to the following [article](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

