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
# <a name="fix-dkim-setup-issues"></a>פתרון בעיות בהגדרת DKIM

אם אתה נתקל בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, בצע את השלבים הבאים:

- רוב בעיות ההגדרה של DKIM קשורות לרשומות DNS שגויות. ודא שרשומת CNAME של DKIM (**לא** רשומת TXT) מעוצבת כראוי. לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)זה.

- לאחר שתיצור או תעדכן את רשומות ה-DNS שלך ב-DKIM בשירות אירוח ה-DNS עבור התחום שלך (בדרך כלל, רשם התחומים שלך), המתן עד שרשומות ה-DNS יופצו.

- אם אינך מצליח ליצור את רשומות ה-DNS של DKIM במרכז הניהול, באפשרותך להחליף \<CustomDomain\> בתחום המותאם אישית שלך (לדוגמה, contoso.com) ולהפעיל פקודה זו ב- [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
