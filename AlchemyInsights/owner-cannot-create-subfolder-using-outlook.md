---
title: הבעלים אינו יכול ליצור תיקיית משנה באמצעות Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836136"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="d70ba-102">הבעלים אינו יכול ליצור תיקיית משנה באמצעות Outlook</span><span class="sxs-lookup"><span data-stu-id="d70ba-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="d70ba-103">**קיימת בעיה מתמשכת עם בעלי תיקיות ציבוריות שיוצרים תיקיות משנה באמצעות Outlook. הבעיה תתוקן בקרוב.**</span><span class="sxs-lookup"><span data-stu-id="d70ba-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="d70ba-104">בינתיים, השתמש באחת מהדרכים הבאות לעקיפת הבעיה:</span><span class="sxs-lookup"><span data-stu-id="d70ba-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="d70ba-105">השתמש ב- Outlook עבור MAC כדי ליצור את תיקיית המשנה כאשר הבעיה משפיעה רק על Outlook עבור חלונות שולחן העבודה (כל הגירסאות)</span><span class="sxs-lookup"><span data-stu-id="d70ba-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="d70ba-106">יש למנהל מערכת ליצור את תיקיית המשנה באמצעות EXO Shell או EAC</span><span class="sxs-lookup"><span data-stu-id="d70ba-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="d70ba-107">שינוי DefaultציבוריFolderMailbox/EffectivePublicFolderMailbox על המשתמש לתיבת דואר אחרת מאשר תיבת הדואר של התוכן עבור התיקיה שגרמה לבעיה</span><span class="sxs-lookup"><span data-stu-id="d70ba-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="d70ba-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="d70ba-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="d70ba-109">המתן שעה, הפעל מחדש את לקוח Outlook</span><span class="sxs-lookup"><span data-stu-id="d70ba-109">Wait for an hour, restart outlook client</span></span>