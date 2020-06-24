---
title: השתמש ב-PowerShell לשיתוף מדיניות וקשרי גומלין בין ארגונים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862087"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>השתמש ב-PowerShell לשיתוף מדיניות וקשרי גומלין בין ארגונים


עבור קשרי גומלין בין ארגונים, עיין בתחביר ובמידע הפרמטרים המפורטים עבור: [מידע מקבל-הפדרלי](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [קשרי גומלין של ארגון חדש](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [קשרי גומלין מוגדרים](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) [והסרת קשר](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)ארגוני.

כדי ליצור שימוש במדיניות שיתוף השתמש [במדיניות חדשה](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)לשיתוף. כדי [להחיל מדיניות שיתוף על תיבת דואר או על משתמש](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) שעליך להשתמש בשילוב של [תיבת דואר](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) [ולקבל תיבת דואר](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) עם המדיניות החדשה שנוצרה. כדי [לשנות, להשבית או להסיר מדיניות שיתוף](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) עליך להשתמש [במדיניות Set-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) [ולהסיר את המדיניות](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**לקבלת הבנה מלאה של נושא זה נא לקרוא:**

[שיתוף ב-Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)