---
title: 929 כללי תיבת הדואר הנכנס ל-הגנה כללים
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724593"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="2481b-102">כללי זרימת דואר (המכונים גם כללי תעבורה)</span><span class="sxs-lookup"><span data-stu-id="2481b-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="2481b-103">מבט כללי על כללי זרימת דואר: [כללי זרימת דואר (כללי תעבורה) ב-Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="2481b-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="2481b-104">הגדרת כללי זרימת דואר: [שגרות כלל זרימת דואר ב-Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="2481b-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="2481b-105">יצירה, שינוי ומחיקה של כללי זרימת דואר: [ניהול כללי זרימת דואר](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="2481b-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="2481b-106">באפשרותך גם לנהל כללי זרימת דואר ב-Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2481b-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="2481b-107">לקבלת מידע נוסף, ראה התחבורה (תצוגה), [התחבורה החדשה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) ( [ליצור](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) ), [הסרה-התחבורה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (למחוק), [הגדרת ההעברה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (לשנות קיים), [השבתת התחבורה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (להשבית את הקיים), ו [-הפעל](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) מחדש (לאפשר קיים).</span><span class="sxs-lookup"><span data-stu-id="2481b-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="2481b-108">יישומוני cmdlet נוספים של כללי זרימת דואר: [מקבל התחבורה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (רשימת פעולות זמינות), [קבל-התחבורה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (רשימת תנאים וחריגים זמינים), [ייצוא התחבורה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (כללי ייצוא), ו [-ייבוא התחבורה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (כללי ייבוא).</span><span class="sxs-lookup"><span data-stu-id="2481b-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
