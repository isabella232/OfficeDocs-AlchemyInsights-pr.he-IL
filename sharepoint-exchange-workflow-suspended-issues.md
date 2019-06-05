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
ms.openlocfilehash: 9a8d72a01ed35794fcab370b48bbb189663d3396
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718748"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="934af-102">זרימות עבודה ב- SharePoint</span><span class="sxs-lookup"><span data-stu-id="934af-102">Workflows in SharePoint</span></span>

<p><span data-ttu-id="934af-103">אם זרימות עבודה של SharePoint לא שולח הודעות דואר אלקטרוני, הארגון שלך נתקל מגבלות השולח Exchange Online.&nbsp;</span><span class="sxs-lookup"><span data-stu-id="934af-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.&nbsp;</span></span></p> <p><span data-ttu-id="934af-104">הודעת השגיאה 'זרימת עבודה מושעית' עלולה להתרחש אם יש לך אחד מהפריטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="934af-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span></p> <ul> <li><span data-ttu-id="934af-105">יש לך זרימת עבודה ב- SharePoint במצב מקוון שבו הוא משתמש SharePoint 2010 או סוג פלטפורמה זרימת עבודה של SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="934af-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span></li> <li><span data-ttu-id="934af-106">זרימת העבודה נקבעה כדי לשלוח הודעת דואר אלקטרוני מותאמות אישית משתמשים יותר מ- 200 בכל פעם, למעלה מ- 10,000 נמענים בכל יום או יותר מ- 30 הודעות לדקה.</span><span class="sxs-lookup"><span data-stu-id="934af-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span></li> <li><span data-ttu-id="934af-107">כאשר אתה מפעיל את זרימת העבודה, לא תישלח הודעת דואר אלקטרוני, אתה מבחין את הודעת השגיאה, מוצג <strong>המצב הפנימי מוגדר מושעה</strong> או <strong>אין אפשרות לשלוח לנמען</strong> .</span><span class="sxs-lookup"><span data-stu-id="934af-107">When you run the workflow, the email message isn't sent, and you notice the error message, <strong>Internal Status is set to Suspended</strong> or <strong>Unable to send to a recipient</strong> is displayed.</span></span></li> </ul> <p><span data-ttu-id="934af-108">לקבלת מידע נוסף, עיין <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">במאמר</a>הבא.</span><span class="sxs-lookup"><span data-stu-id="934af-108">For more information, please refer to the following <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">article</a>.</span></span></p>

