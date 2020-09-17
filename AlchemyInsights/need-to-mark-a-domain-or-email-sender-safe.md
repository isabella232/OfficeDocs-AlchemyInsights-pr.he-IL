---
title: צריך לסמן תחום או שולח דואר אלקטרוני בטוח?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803246"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="1a8b9-102">צריך לסמן תחום או שולח דואר אלקטרוני בטוח?</span><span class="sxs-lookup"><span data-stu-id="1a8b9-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="1a8b9-103">שימוש **ברשימות שולחים בטוחים אינו מומלץ מאחר** שהוא פותח את הארגון שלך להודעות זבל, פיש וזיופים.</span><span class="sxs-lookup"><span data-stu-id="1a8b9-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="1a8b9-104">עם זאת, אם קיימת דרישה עסקית, אנו **ממליצים** להשתמש **[בכללי זרימת דואר](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** עבור פעולה זו.</span><span class="sxs-lookup"><span data-stu-id="1a8b9-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="1a8b9-105">ההדרכה שלנו מבטיחה אימות שולח (אימות התחום השולח אינו מזויף).</span><span class="sxs-lookup"><span data-stu-id="1a8b9-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="1a8b9-106">**הערה**: אנו לא ממליצים על ניהול חיובים שקריים באמצעות רשימות שולחים בטוחים, מאחר שחריגים לסינון הודעות זבל יכולים לפתוח את הארגון שלך להתקפות אבטחה.</span><span class="sxs-lookup"><span data-stu-id="1a8b9-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="1a8b9-107">אם המשתמש שלך מקבל הודעות המסומנות באופן שגוי כדואר זבל או דואר זבל, **[דווח על הודעות וקבצים ל-Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="1a8b9-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="1a8b9-108">שולחים בטוחים ב-Outlook, ברשימת השולחים המותרים או ברשימת התחומים המותרים במדיניות למניעת הודעות זבל **יש להימנע** מכיוון ששולחים עוקפים את כל הודעות הדואר האלקטרוני, הזיופים והפיש ואימות השולח (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="1a8b9-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="1a8b9-109">מומלץ להשתמש בשיטה זו לבדיקה זמנית בלבד.</span><span class="sxs-lookup"><span data-stu-id="1a8b9-109">This method is best used for temporary testing only.</span></span>
