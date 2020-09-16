---
title: לבעלים אין אפשרות ליצור תיקיית משנה באמצעות Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665719"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="8ca0b-102">לבעלים אין אפשרות ליצור תיקיית משנה באמצעות Outlook</span><span class="sxs-lookup"><span data-stu-id="8ca0b-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="8ca0b-103">**קיימת בעיה מתמשכת עם בעלי תיקיות ציבוריות שיוצרים תיקיות משנה באמצעות Outlook. הבעיה תתוקן בקרוב.**</span><span class="sxs-lookup"><span data-stu-id="8ca0b-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="8ca0b-104">בינתיים, השתמש באחת מהפתרונות הבאים:</span><span class="sxs-lookup"><span data-stu-id="8ca0b-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="8ca0b-105">שימוש ב-Outlook עבור MAC כדי ליצור את תיקיית המשנה כבעיה משפיעה רק על Outlook עבור windows desktop (כל הגירסאות)</span><span class="sxs-lookup"><span data-stu-id="8ca0b-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="8ca0b-106">ניהול מנהל המערכת צור את תיקיית המשנה באמצעות קליפת Shell או EAC</span><span class="sxs-lookup"><span data-stu-id="8ca0b-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="8ca0b-107">שינוי הDefaultPublicFolderMailbox/EffectivePublicFolderMailbox במשתמש לתיבת דואר אחרת מאשר תיבת הדואר של התוכן עבור הבעיה הגורמת לתיקיה</span><span class="sxs-lookup"><span data-stu-id="8ca0b-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="8ca0b-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="8ca0b-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="8ca0b-109">המתן לשעה, הפעל מחדש את לקוח outlook</span><span class="sxs-lookup"><span data-stu-id="8ca0b-109">Wait for an hour, restart outlook client</span></span>