---
title: פתרון בעיות של Office 365 להגנה על איומים מתקדמים
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 7391b3c126d55213881f6b71cb6b5fc72bc68d0f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512591"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="137c1-102">פתרון בעיות של Office 365 להגנה על איומים מתקדמים</span><span class="sxs-lookup"><span data-stu-id="137c1-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="137c1-103">האם אתה מבחין בעיכובים? במסירת הודעות</span><span class="sxs-lookup"><span data-stu-id="137c1-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="137c1-104">השתמש באפשרות ' [מסירה דינאמית](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) ' במדיניות ' קבצים מצורפים בטוחים של ATP '.</span><span class="sxs-lookup"><span data-stu-id="137c1-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="137c1-105">פעולה זו תסייע למנוע עיכובים בהודעות בעת הגנה על נמענים מפני קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="137c1-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="137c1-106">האם ברצונך לדווח ל-Microsoft על תוצאות חיוביות שגויות או על שליליות מזויפות?</span><span class="sxs-lookup"><span data-stu-id="137c1-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="137c1-107">השתמש [בקישור](https://www.microsoft.com/wdsi/filesubmission/) זה כדי לשלוח קבצים לניתוח.</span><span class="sxs-lookup"><span data-stu-id="137c1-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="137c1-108">האם ידעת שבאפשרותך לאפשר הגנה מפני קישורים בטוחים עבור דואר אלקטרוני פנימי שנשלח בין הנמענים בארגון?</span><span class="sxs-lookup"><span data-stu-id="137c1-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="137c1-109">בצע שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="137c1-109">Follow these steps:</span></span>

  1. <span data-ttu-id="137c1-110">עבור אל https://protection.office.com והיכנס למערכת כללית או לחשבון מנהל האבטחה.</span><span class="sxs-lookup"><span data-stu-id="137c1-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="137c1-111">בחלונית הניווט השמאלית תחת **ניהול איומים**, בחר באפשרות קישורים בטוחים **של מדיניות** \> **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="137c1-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="137c1-112">בפריטי **המדיניות החלים על המקטע הארגוני כולו** , בחר את המדיניות ולחץ על **Edit**.</span><span class="sxs-lookup"><span data-stu-id="137c1-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="137c1-113">תחת **הגדרות**, הפעל **את האפשרות החל קישורים בטוחים על הודעות הנשלחות בארגון**.</span><span class="sxs-lookup"><span data-stu-id="137c1-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
