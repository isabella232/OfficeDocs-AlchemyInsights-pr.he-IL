---
title: פתרון בעיות ב- Microsoft Defender עבור Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545269"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="16d69-102">פתרון בעיות ב- Microsoft Defender עבור Office 365</span><span class="sxs-lookup"><span data-stu-id="16d69-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="16d69-103">**האם אתה מבחין בעיכובים במסירת הודעות?**</span><span class="sxs-lookup"><span data-stu-id="16d69-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="16d69-104">השתמש באפשרות [מסירה דינאמית](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) במדיניות Microsoft Defender Office 365 קבצים מצורפים בטוחים.</span><span class="sxs-lookup"><span data-stu-id="16d69-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="16d69-105">פעולה זו תסייע למנוע עיכובים בהודעות בעת הגנה על נמענים מפני קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="16d69-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="16d69-106">**האם ברצונך הדוח חיוביים או שליליים שגויים ל- Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="16d69-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="16d69-107">השתמש [בסייר ההגשות.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="16d69-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="16d69-108">-\*\* האם ידעת שתוכל להפוך הגנה על קישורים בטוחים לזמינה עבור דואר אלקטרוני פנימי שנשלח בין הנמענים בארגון שלך?\*\* בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="16d69-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="16d69-109">עבור אל [https://protection.office.com](https://protection.office.com) והירשם באמצעות חשבון מנהל מערכת כללי או מנהל אבטחה.</span><span class="sxs-lookup"><span data-stu-id="16d69-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="16d69-110">בחלונית הניווט הימנית תחת **ניהול איומים**, בחר **קישורים בטוחים** של \> **מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="16d69-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="16d69-111">במקטע **פריטי מדיניות החלים על הארגון כולו,** בחר את המדיניות ולחץ על **ערוך**.</span><span class="sxs-lookup"><span data-stu-id="16d69-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="16d69-112">תחת **הגדרות,** הפוך **את האפשרות החל קישורים בטוחים על הודעות הנשלחות בתוך הארגון.**</span><span class="sxs-lookup"><span data-stu-id="16d69-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
