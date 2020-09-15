---
title: תחילת העבודה עם SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700708"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="e05ab-102">זרימות עבודה ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="e05ab-102">Workflows in SharePoint</span></span>

<span data-ttu-id="e05ab-103">אם זרימות עבודה של SharePoint אינן שולחות הודעות דואר אלקטרוני, ייתכן שהארגון שלך נתקל במגבלות השולח של Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e05ab-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="e05ab-104">הודעת השגיאה ' זרימת עבודה מושעית ' עשויה להתרחש אם יש לך אחד מהפריטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e05ab-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="e05ab-105">יש לך זרימת עבודה ב-SharePoint Online המשתמשת בסוג פלטפורמת זרימת העבודה של SharePoint 2010 או SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="e05ab-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="e05ab-106">זרימת העבודה מוגדרת לשליחת הודעת דואר אלקטרוני מותאמת אישית ליותר מ-200 משתמשים בכל פעם, יותר מ-10,000 נמענים לכל יום, או יותר מ-30 הודעות בדקה.</span><span class="sxs-lookup"><span data-stu-id="e05ab-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="e05ab-107">כאשר אתה מפעיל את זרימת העבודה, הודעת הדואר האלקטרוני אינה נשלחת, ואתה מבחין בהודעת השגיאה, המצב הפנימי מוגדר כמושהה או שאין אפשרות לשלוח לנמען מוצג.</span><span class="sxs-lookup"><span data-stu-id="e05ab-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="e05ab-108">לקבלת מידע נוסף, עיין [במאמר](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)הבא.</span><span class="sxs-lookup"><span data-stu-id="e05ab-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

