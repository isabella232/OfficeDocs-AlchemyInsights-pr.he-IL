---
title: תקן בעיות התקנה של DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506775"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="e8dc0-102">תקן בעיות התקנה של DKIM</span><span class="sxs-lookup"><span data-stu-id="e8dc0-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="e8dc0-103">אם נתקלת בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, השתמש בשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e8dc0-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="e8dc0-104">רוב בעיות ההתקנה של DKIM קשורות לרשומות DNS שגויות.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="e8dc0-105">ודא שרשומת ה-DKIM CNAME (**לא** רשומת TXT) מעוצבת כראוי.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="e8dc0-106">לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)זה.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="e8dc0-107">לאחר שתיצור או תעדכן את רשומות DKIM DNS שלך בשירות DNS המארח עבור התחום שלך (בדרך כלל, רשם התחום שלך), המתן עד שרשומות ה-DNS יהיו מופצות.</span><span class="sxs-lookup"><span data-stu-id="e8dc0-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="e8dc0-108">אם אינך מצליח ליצור את רשומות DKIM DNS במרכז הניהול, באפשרותך להחליף את \<CustomDomain\> התחום המותאם אישית שלך (לדוגמה, contoso.com) ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="e8dc0-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
