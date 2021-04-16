---
title: האם עליך לסמן תחום או שולח דואר אלקטרוני בטוחים?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792133"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="64b2e-102">האם עליך לסמן תחום או שולח דואר אלקטרוני בטוחים?</span><span class="sxs-lookup"><span data-stu-id="64b2e-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="64b2e-103">השימוש **ברשימות שולחים בטוחים אינו מומלץ** מאחר שהוא פותח את הארגון שלך כדי לשלוח הודעות זבל, דיוג ותקפות תוקף.</span><span class="sxs-lookup"><span data-stu-id="64b2e-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="64b2e-104">עם זאת, אם יש דרישה עסקית, מומלץ **להשתמש** **[בכללי זרימת דואר](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** עבור פעולה זו.</span><span class="sxs-lookup"><span data-stu-id="64b2e-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="64b2e-105">ההנחיות שלנו מבטיחות אימות שולח (מוודאת שלא תפורסם שליחה של תחום).</span><span class="sxs-lookup"><span data-stu-id="64b2e-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="64b2e-106">**הערה:** איננו ממליצים לנהל תוצאות חיוביות שגויות באמצעות רשימות שולחים בטוחים, מכיוון שחסכון חריג לסינון דואר זבל יכול לפתוח את הארגון שלך להתקפות אבטחה.</span><span class="sxs-lookup"><span data-stu-id="64b2e-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="64b2e-107">אם המשתמשים שלך מקבלים הודעות המסומנות באופן שגוי כדואר זבל או כדואר זבל, **[דווח על הודעות וקבצים ל- Microsoft.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="64b2e-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="64b2e-108">יש להימנע משולחים בטוחים ב- Outlook, ברשימת שולחים מותרים או ברשימת תחומים מותרים במדיניות למניעת דואר זבל מכיוון ששולחים עוקפים את כל הודעות הזבל, התחנפות וההגנה מפני דיוג ואימות שולח (SPF, DKIM, DMARC). </span><span class="sxs-lookup"><span data-stu-id="64b2e-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="64b2e-109">שיטה זו משמשת באופן הטוב ביותר לבדיקות זמניות בלבד.</span><span class="sxs-lookup"><span data-stu-id="64b2e-109">This method is best used for temporary testing only.</span></span>
