---
title: פתרון בעיות בהגדרת DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744951"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="6caf4-102">פתרון בעיות בהגדרת DKIM</span><span class="sxs-lookup"><span data-stu-id="6caf4-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="6caf4-103">אם אתה נתקל בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="6caf4-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="6caf4-104">רוב בעיות ההגדרה של DKIM קשורות לרשומות DNS שגויות.</span><span class="sxs-lookup"><span data-stu-id="6caf4-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="6caf4-105">ודא שרשומת CNAME של DKIM (**לא** רשומת TXT) מעוצבת כראוי.</span><span class="sxs-lookup"><span data-stu-id="6caf4-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6caf4-106">לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)זה.</span><span class="sxs-lookup"><span data-stu-id="6caf4-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="6caf4-107">לאחר שתיצור או תעדכן את רשומות ה-DNS שלך ב-DKIM בשירות אירוח ה-DNS עבור התחום שלך (בדרך כלל, רשם התחומים שלך), המתן עד שרשומות ה-DNS יופצו.</span><span class="sxs-lookup"><span data-stu-id="6caf4-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="6caf4-108">אם אינך מצליח ליצור את רשומות ה-DNS של DKIM במרכז הניהול, באפשרותך להחליף \<CustomDomain\> בתחום המותאם אישית שלך (לדוגמה, contoso.com) ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="6caf4-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
