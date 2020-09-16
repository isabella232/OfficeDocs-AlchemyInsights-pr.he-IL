---
title: הודעות ההתראה של SharePoint שלא נמסרו
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751244"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="d1438-102">הודעות ההתראה של SharePoint שלא נמסרו</span><span class="sxs-lookup"><span data-stu-id="d1438-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="d1438-103">בדוק את תיקיית דואר הזבל בהודעת הדואר האלקטרוני שלך, כפי שלפעמים התראות עשויות להיכנס לשם.</span><span class="sxs-lookup"><span data-stu-id="d1438-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="d1438-104">קבע אם **כל ההתראות לא יועברו** או אם **התראה בודדת** מקובץ או ספריה ספציפית לא נמסר.</span><span class="sxs-lookup"><span data-stu-id="d1438-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="d1438-105">**התראות בודדות אינן מועברות**: אם התראה בודדת מקובץ או ספריה ספציפית לא נמסר, באפשרותך לנסות למחוק אותו וליצור אותו מחדש.</span><span class="sxs-lookup"><span data-stu-id="d1438-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="d1438-106">ראה [ניהול, הצגה או מחיקה של התראות](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) ב-SharePoint כדי ליצור מחדש את ההתראה.</span><span class="sxs-lookup"><span data-stu-id="d1438-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="d1438-107">**כל ההתראות לא נמסרות**: אם כל ההתראות מקבצים או ספריות מרובות אינם מועברים, בקר [בלוח המחוונים של תקינות השירות](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק את כל העלונים/האירועים שעשויים להתרחש באמצעות SharePoint או Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1438-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="d1438-108">הבעיה עשויה להיות עם יכולת ההתראה של SharePoint או עיכובים בהודעות דואר אלקטרוני באמצעות Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1438-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="d1438-109">חשוב גם לציין אם דואר אלקטרוני אחר מועבר, ואם לא, סביר להניח שהבעיה היא עיכובים של Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1438-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="d1438-110">שאלות נפוצות בנושא התראות:</span><span class="sxs-lookup"><span data-stu-id="d1438-110">FAQ on alerts:</span></span>

- <span data-ttu-id="d1438-111">לא ניתן לשלוח התראות לקבוצת תפוצה, רק קבוצות אבטחה וO365 נתמכות.</span><span class="sxs-lookup"><span data-stu-id="d1438-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="d1438-112">אין באפשרותך להתאים אישית תבניות דואר אלקטרוני של התראות; עליך להשתמש בזרימת העבודה של Microsoft FLOW או ב-SharePoint Designer כדי להשיג אותם.</span><span class="sxs-lookup"><span data-stu-id="d1438-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="d1438-113">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="d1438-113">Related Topics</span></span>

<span data-ttu-id="d1438-114">מעוניין לנסות את Microsoft Flow ב-SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="d1438-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="d1438-115">יצירת זרימה</span><span class="sxs-lookup"><span data-stu-id="d1438-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="d1438-116">SharePoint ו-Flow</span><span class="sxs-lookup"><span data-stu-id="d1438-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
