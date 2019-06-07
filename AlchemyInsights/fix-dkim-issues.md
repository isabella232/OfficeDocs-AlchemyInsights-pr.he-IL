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
# <a name="fix-dkim-setup-issues"></a>לפתור בעיות התקנה של DKIM

אם אתה נתקל בבעיות הפעלה DKIM עבור התחום המותאם אישית שלך, בצע את הפעולות הבאות:

- רוב בעיות ההתקנה DKIM הקשורות לרשומות ה-DNS שגויה. ודא שרשומת DKIM CNAME (**לא** רשומה TXT) מעוצב כראוי. לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)זה.

- לאחר ליצור או לעדכן רשומות DKIM DNS שלך ב- DNS המארח שירות עבור התחום שלך (בדרך כלל, שלך רשם תחום), המתן להפיץ רשומות DNS.

- אם אין באפשרותך ליצור רשומות ה-DNS DKIM במרכז admin, באפשרותך להחליף את \<CustomDomain\> עם התחום המותאם אישית שלך (לדוגמה, contoso.com) ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
