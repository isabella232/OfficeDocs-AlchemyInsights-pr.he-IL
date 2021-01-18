---
title: הצהרת SAML (אסימונים)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885215"
---
# <a name="saml-assertions-tokens"></a>הצהרת SAML (אסימונים)

1. האסימונים של ' הצהרות אבטחה ' (SAML) הם ייצוגי XML של טענות. כברירת מחדל, משתמשים ב-SAML tokens של יסודות התקשורת של Windows (WCF) בתרחישים של אבטחה מאוחדת מונפקים אסימונים. לקבלת מידע נוסף, ראה [אסימונים וטענות של SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. פלטפורמת הזהויות של Microsoft פולטת כמה סוגים של אסימוני אבטחה בעיבוד של כל זרימת אימות. [הפניה לטענות אסימון SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) מתארת את העיצוב, מאפייני האבטחה והתוכן של SAML 2.0.
3. פעל לפי ההנחיות [באורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) כדי להבין כיצד לקבוע אורך חיים של אסימונים.
4. בצע את השלבים המתוארים [במאמר זה](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) כדי להבין כיצד לקבוע את התצורה של הצפנת אסימון מסוג תכלת AD SAML.
5. ב-תכלת לספירה, באפשרותך להגדיר אפשרויות חתימת אישורים ואת אלגוריתם חתימת האישורים. לקבלת מידע נוסף, ראה [אפשרויות של חתימת אישורים מתקדמת באסימון SAML עבור יישומי גלריה ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
