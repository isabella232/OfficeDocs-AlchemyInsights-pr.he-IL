---
title: לפתור בעיות התקנה של DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765109"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="823b7-102">לפתור בעיות התקנה של DKIM</span><span class="sxs-lookup"><span data-stu-id="823b7-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="823b7-103">אם אתה נתקל בבעיות הפעלה DKIM עבור התחום המותאם אישית שלך, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="823b7-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="823b7-104">רוב בעיות ההתקנה DKIM הקשורות לרשומות ה-DNS שגויה.</span><span class="sxs-lookup"><span data-stu-id="823b7-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="823b7-105">ודא שרשומת DKIM CNAME (**לא** רשומה TXT) מעוצב כראוי.</span><span class="sxs-lookup"><span data-stu-id="823b7-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="823b7-106">לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)זה.</span><span class="sxs-lookup"><span data-stu-id="823b7-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="823b7-107">לאחר ליצור או לעדכן רשומות DKIM DNS שלך ב- DNS המארח שירות עבור התחום שלך (בדרך כלל, שלך רשם תחום), המתן להפיץ רשומות DNS.</span><span class="sxs-lookup"><span data-stu-id="823b7-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="823b7-108">אם אין באפשרותך ליצור רשומות ה-DNS DKIM במרכז admin, באפשרותך להחליף את \<CustomDomain\> עם התחום המותאם אישית שלך (לדוגמה, contoso.com) ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="823b7-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
