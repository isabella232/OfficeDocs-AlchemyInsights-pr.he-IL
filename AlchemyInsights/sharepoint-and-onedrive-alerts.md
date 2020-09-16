---
title: עיכובים בקבלת התראות של SharePoint ו-OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727244"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="5231e-102">עיכובים בקבלת התראות של SharePoint ו-OneDrive</span><span class="sxs-lookup"><span data-stu-id="5231e-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="5231e-103">תחילה, בדוק את התיקיה ' זבל ' או ' דואר זבל ' בדואר האלקטרוני שלך.</span><span class="sxs-lookup"><span data-stu-id="5231e-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="5231e-104">אם **כל ההתראות מקבצים או ספריות מרובות מעוכבות**, בקר [בלוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home?ref=/servicehealth) כדי לבדוק את כל התקריות/האירועים שעשויים להתרחש באמצעות SharePoint או Exchange.</span><span class="sxs-lookup"><span data-stu-id="5231e-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="5231e-105">הבעיה עשויה להיות עם יכולת ההתראה של SharePoint או עיכובים בהודעות דואר אלקטרוני באמצעות Exchange.</span><span class="sxs-lookup"><span data-stu-id="5231e-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="5231e-106">כמו כן, שים לב אם דואר אלקטרוני אחר מועבר-אם לא, סביר להניח שהבעיה היא עיכובים של Exchange.</span><span class="sxs-lookup"><span data-stu-id="5231e-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="5231e-107">אם **התראה בודדת מקובץ או ספריה ספציפית אינו מועבר**, נסה למחוק אותה וליצור אותה מחדש.</span><span class="sxs-lookup"><span data-stu-id="5231e-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="5231e-108">ראה [ניהול, הצגה או מחיקה של התראות](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) ב-SharePoint כדי ליצור מחדש את ההתראה.</span><span class="sxs-lookup"><span data-stu-id="5231e-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="5231e-109">לא ניתן לשלוח התראות לקבוצת תפוצה.</span><span class="sxs-lookup"><span data-stu-id="5231e-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="5231e-110">רק קבוצות אבטחה וO365 נתמכות.</span><span class="sxs-lookup"><span data-stu-id="5231e-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="5231e-111">אין באפשרותך להתאים אישית תבניות דואר אלקטרוני של התראה.</span><span class="sxs-lookup"><span data-stu-id="5231e-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="5231e-112">עליך להשתמש בזרימת העבודה של Microsoft Flow או ב-SharePoint Designer כדי להשיג אותם.</span><span class="sxs-lookup"><span data-stu-id="5231e-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
