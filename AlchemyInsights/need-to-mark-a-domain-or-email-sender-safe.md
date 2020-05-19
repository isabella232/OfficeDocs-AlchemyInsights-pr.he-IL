---
title: צריך לסמן תחום או שולח דוא ל בטוח?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281149"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="888e7-102">צריך לסמן תחום או שולח דוא ל בטוח?</span><span class="sxs-lookup"><span data-stu-id="888e7-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="888e7-103">**שימוש ברשימות שולח בטוחות אינו מומלץ מאחר** שהוא פותח את הארגון שלך לדואר זבל, phish והתקפות זיופים.</span><span class="sxs-lookup"><span data-stu-id="888e7-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="888e7-104">עם זאת, אם קיימת דרישה עסקית, אנו **ממליצים** להשתמש **[בכללי זרימת דואר](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** עבור פעולה זו.</span><span class="sxs-lookup"><span data-stu-id="888e7-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="888e7-105">ההנחיה שלנו מבטיחה אימות שולח (מוודא ששליחת קבוצת מחשבים אינה מתחזה).</span><span class="sxs-lookup"><span data-stu-id="888e7-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="888e7-106">**הערה**: אנו לא ממליצים על ניהול תוצאות חיוביות כוזבות באמצעות רשימות שולח בטוחות, מכיוון שחריגים לסינון דואר זבל יכולים לפתוח את הארגון שלך להתקפות אבטחה.</span><span class="sxs-lookup"><span data-stu-id="888e7-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="888e7-107">אם המשתמש שלך מקבל הודעות המסומנות באופן שגוי כדואר זבל או כדואר זבל, **[דווח למיקרוסופט על הודעות וקבצים](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="888e7-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="888e7-108">**יש להימנע** משולחים בטוחים ב-Outlook, רשימת שולחים מותרים, או רשימת תחומים המותרים במדיניות נגד דואר זבל, מכיוון ששולחים עוקפים את כל הודעות הזבל, הפרודיה וההגנה של פיש ואימות השולח (SPF, dkim, dkim).</span><span class="sxs-lookup"><span data-stu-id="888e7-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="888e7-109">שיטה זו משמשת באופן הטוב ביותר לבדיקה זמנית בלבד.</span><span class="sxs-lookup"><span data-stu-id="888e7-109">This method is best used for temporary testing only.</span></span>
