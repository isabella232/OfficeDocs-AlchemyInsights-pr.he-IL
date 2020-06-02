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
# <a name="fix-dkim-setup-issues"></a>תקן בעיות התקנה של DKIM

אם נתקלת בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, השתמש בשלבים הבאים:

- רוב בעיות ההתקנה של DKIM קשורות לרשומות DNS שגויות. ודא שרשומת ה-DKIM CNAME (**לא** רשומת TXT) מעוצבת כראוי. לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)זה.

- לאחר שתיצור או תעדכן את רשומות DKIM DNS שלך בשירות DNS המארח עבור התחום שלך (בדרך כלל, רשם התחום שלך), המתן עד שרשומות ה-DNS יהיו מופצות.

- אם אינך מצליח ליצור את רשומות DKIM DNS במרכז הניהול, באפשרותך להחליף את \<CustomDomain\> התחום המותאם אישית שלך (לדוגמה, contoso.com) ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
