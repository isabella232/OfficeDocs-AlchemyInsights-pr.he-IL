---
title: SAML Assertions (Tokens)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109241"
---
# <a name="saml-assertions-tokens"></a>SAML Assertions (Tokens)

1. אסימוני שפת סימון של ערכות אבטחה (SAML) הם ייצוגי XML של תביעות. כברירת מחדל, אסימוני SAML Windows Communication Foundation (WCF) משתמשים בתרחישי אבטחה מאוחדים הם אסימונים שהונפקו. לקבלת מידע נוסף, ראה [אסימוני SAML ותביעות](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. ה פלטפורמת הזהויות של Microsoft פולט כמה סוגים של אסימוני אבטחה בעיבוד של כל זרימת אימות. [חומר עזר של תביעות אסימון SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) מתאר את התבנית, מאפייני האבטחה והתוכן של אסימוני SAML 2.0.
3. בצע את ההנחיות [בתקופות חיים של אסימון הניתן להגדרה פלטפורמת הזהויות של Microsoft להבין](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) כיצד לקבוע את התצורה של משך חיים של אסימון.
4. בצע את השלבים המתוארים במאמר [זה כדי להבין](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) כיצד להגדיר הצפנת אסימון של Azure AD SAML.
5. ב- Azure AD, באפשרותך להגדיר אפשרויות חתימת אישורים ואלגוריתם חתימת האישורים. לקבלת מידע נוסף, ראה אפשרויות [מתקדמות של חתימת אישורים באסימון SAML עבור יישומי גלריה ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
