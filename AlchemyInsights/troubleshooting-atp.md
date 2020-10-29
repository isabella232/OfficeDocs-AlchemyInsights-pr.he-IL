---
title: פתרון בעיות של Microsoft Defender עבור Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801444"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="7a15b-102">פתרון בעיות של Microsoft Defender עבור Office 365</span><span class="sxs-lookup"><span data-stu-id="7a15b-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="7a15b-103">האם אתה מבחין בעיכובים במסירת הודעות?</span><span class="sxs-lookup"><span data-stu-id="7a15b-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="7a15b-104">השתמש באפשרות [המסירה הדינאמית](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) במדיניות הקבצים המצורפים הבטוחים של ATP.</span><span class="sxs-lookup"><span data-stu-id="7a15b-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="7a15b-105">פעולה זו תעזור למנוע עיכובים של הודעות תוך הגנה על נמענים מקבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="7a15b-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="7a15b-106">האם ברצונך לדווח על חיובים כוזבים או שליליות false ל-Microsoft?</span><span class="sxs-lookup"><span data-stu-id="7a15b-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="7a15b-107">השתמש [בקישור](https://www.microsoft.com/wdsi/filesubmission/) זה כדי לשלוח קבצים לניתוח.</span><span class="sxs-lookup"><span data-stu-id="7a15b-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="7a15b-108">האם ידעת שבאפשרותך להפעיל הגנה על קישורים בטוחים עבור דואר אלקטרוני פנימי שנשלח בין נמענים בארגון שלך?</span><span class="sxs-lookup"><span data-stu-id="7a15b-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="7a15b-109">בצע שלבים אלה:</span><span class="sxs-lookup"><span data-stu-id="7a15b-109">Follow these steps:</span></span>

  1. <span data-ttu-id="7a15b-110">עבור אל [https://protection.office.com](https://protection.office.com) והיכנס באמצעות חשבון מנהל מערכת כללי או מנהל אבטחה.</span><span class="sxs-lookup"><span data-stu-id="7a15b-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="7a15b-111">בחלונית הניווט הימנית תחת **ניהול האיום** , בחר באפשרות קישורים בטוחים **של מדיניות** \> **Safe Links** .</span><span class="sxs-lookup"><span data-stu-id="7a15b-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="7a15b-112">בפריטי **המדיניות החלים על המקטע כולו של הארגון** , בחר את המדיניות ולחץ על **ערוך** .</span><span class="sxs-lookup"><span data-stu-id="7a15b-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="7a15b-113">תחת **הגדרות** , הפעל את **האפשרות החל קישורים בטוחים על הודעות הנשלחות בתוך הארגון** .</span><span class="sxs-lookup"><span data-stu-id="7a15b-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
