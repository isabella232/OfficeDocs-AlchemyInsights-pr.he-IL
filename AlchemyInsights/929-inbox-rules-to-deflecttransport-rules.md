---
title: כללי תיבת דואר נכנס 929 על כללי deflectTransport
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 45c542191dd5ef67cef464e1f204358471c21948
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29928585"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="17277-102">כללי זרימת דואר (המכונה גם כללי תעבורה)</span><span class="sxs-lookup"><span data-stu-id="17277-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="17277-103">מבט כולל על כללי זרימת דואר: [דואר זרימה כללים (תעבורה כללים) ב- Exchange באופן מקוון](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="17277-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>
    
- <span data-ttu-id="17277-104">הגדרת כללי זרימת דואר: [דואר זרימה הליכים כלל ב- Exchange באופן מקוון](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="17277-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>
    
- <span data-ttu-id="17277-105">יצירה, שינוי ומחיקה של כללי זרימת דואר: [ניהול כללי של זרימת דואר](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="17277-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>
    
<span data-ttu-id="17277-p101">באפשרותך גם לנהל כללי זרימת דואר ב- Exchange Online PowerShell. לקבלת מידע נוסף, ראה [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (תצוגה), [TransportRule חדש](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (צור), [TransportRule הסרה](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (מחיקה), [קבוצת-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (שינוי קיים), [TransportRule הפוך ללא זמין](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable קיימים), ו- [אפשר-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (הקיימת לזמינה).</span><span class="sxs-lookup"><span data-stu-id="17277-p101">You can also manage mail flow rules in Exchange Online PowerShell. For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span> 
  
<span data-ttu-id="17277-108">כלי cmdlet של כלל זרימת דואר נוספים: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (רשימת פעולות זמינות), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (רשימה זמינה ותנאים חריגים), [ייצוא-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (ייצוא כללים) ו- [ ייבוא-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (ייבוא כללי).</span><span class="sxs-lookup"><span data-stu-id="17277-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span> 
  

