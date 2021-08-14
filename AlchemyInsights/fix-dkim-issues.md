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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945932"
---
# <a name="fix-dkim-setup-issues"></a>פתרון בעיות בהגדרת DKIM

אם אתה נתקל בבעיות המאפשרות DKIM עבור התחום המותאם אישית שלך, בצע את השלבים הבאים:

- רוב בעיות ההגדרה של DKIM קשורות ברשומות DNS שגויות. ודא כי רשומת CNAME של DKIM **(** לא רשומת TXT) מעוצבת כראוי. לקבלת מידע נוסף, עיין בנושא [זה](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- לאחר יצירה או עדכון של רשומות ה- DNS של DKIM בשירות אירוח ה- DNS עבור התחום שלך (בדרך כלל, רשם התחומים שלך), המתן להפצת רשומות ה- DNS.

- אם אינך יכול ליצור את רשומות ה- DNS של DKIM במרכז הניהול, באפשרותך להחליף בתחום המותאם אישית \<CustomDomain\> שלך (לדוגמה, contoso.com) ולהפעיל [פקודה זו ב- Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
