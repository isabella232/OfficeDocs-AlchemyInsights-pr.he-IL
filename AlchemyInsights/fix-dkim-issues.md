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
# <a name="fix-dkim-setup-issues"></a>תקן בעיות התקנה של DKIM

אם נתקלת בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, השתמש בשלבים הבאים:

- רוב בעיות ההתקנה של DKIM קשורות לרשומות DNS שגויות. ודא שרשומת ה-DKIM CNAME (**לא** רשומת TXT) מעוצבת כראוי. לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)זה.

- לאחר שתיצור או תעדכן את רשומות DKIM DNS שלך בשירות DNS המארח עבור התחום שלך (בדרך כלל, רשם התחום שלך), המתן עד שרשומות ה-DNS יהיו מופצות.

- אם אין באפשרותך ליצור את רשומות ה-DNS של DKIM במרכז \<הניהול,\> תוכל להחליף את תחום ההתאמה האישית עם התחום שלך (לדוגמה, contoso.com) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):.
