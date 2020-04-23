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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717563"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="1f197-102">תקן בעיות התקנה של DKIM</span><span class="sxs-lookup"><span data-stu-id="1f197-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="1f197-103">אם נתקלת בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, השתמש בשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1f197-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="1f197-104">רוב בעיות ההתקנה של DKIM קשורות לרשומות DNS שגויות.</span><span class="sxs-lookup"><span data-stu-id="1f197-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="1f197-105">ודא שרשומת ה-DKIM CNAME (**לא** רשומת TXT) מעוצבת כראוי.</span><span class="sxs-lookup"><span data-stu-id="1f197-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="1f197-106">לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)זה.</span><span class="sxs-lookup"><span data-stu-id="1f197-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="1f197-107">לאחר שתיצור או תעדכן את רשומות DKIM DNS שלך בשירות DNS המארח עבור התחום שלך (בדרך כלל, רשם התחום שלך), המתן עד שרשומות ה-DNS יהיו מופצות.</span><span class="sxs-lookup"><span data-stu-id="1f197-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="1f197-108">אם אין באפשרותך ליצור את רשומות ה-DNS של DKIM במרכז \<הניהול,\> תוכל להחליף את תחום ההתאמה האישית עם התחום שלך (לדוגמה, contoso.com) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):.</span><span class="sxs-lookup"><span data-stu-id="1f197-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
