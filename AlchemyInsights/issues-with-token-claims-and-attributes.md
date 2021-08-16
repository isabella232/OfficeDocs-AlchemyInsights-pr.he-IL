---
title: בעיות עם תביעות ותכונות של אסימון
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012885"
---
# <a name="issues-with-token-claims-and-attributes"></a>בעיות עם תביעות ותכונות של אסימון

**עדכון, קביעת תצורה או הסרה של תביעות אסימון**

1. באמצעות Azure Active Directory (Azure [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) AD), באפשרותך להתאים אישית את סוג התביעה עבור תביעת התפקיד באסימון התגובה שאתה מקבל לאחר אישור יישום.
2. מפתחי יישומים יכולים להשתמש בתביעות אופציונליות ביישום Azure AD שלהם כדי לציין אילו טענות הם רוצים באסימונים הנשלחים ליישום שלהם. לקבלת מידע נוסף, ראה [מתן תביעות אופציונליות לאפליקציה שלך](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [קביעת תצורה של תביעות קבוצה עבור יישומים באמצעות Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. אם אתה משתמש ב'כניסה יחידה חלקה' ביישום שלך, ראה התאמה אישית של תביעות שהונפקו [באסימון SAML עבור יישומים ארגוניים](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**מיפוי תכונות טענות**

1. כדי לקבוע את התצורה של מדיניות מיפוי תביעות באמצעות PowerShell, ראה התאמה אישית של תביעות שהופצו [באסימונים עבור יישום ספציפי דייר (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. תכונות הרחבת סכימה של מדריך כתובות מספקות דרך לאחסן נתונים נוספים ב- Azure Active Directory באובייקטי משתמש ובאובייקטים אחרים של מדריך כתובות, כגון קבוצות, פרטי דיירים, מנהלי שירות. ניתן להשתמש רק בתכונות הרחבה באובייקטי משתמש להפלטת תביעות ליישומים. [שימוש בתכונות ההרחבה של סכימת מדריך הכתובות בתביעות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) מתאר כיצד להשתמש בתכונות הרחבת סכימת מדריך כתובות לשליחת נתוני משתמשים ליישומים בתביעות אסימון.

לקבלת מידע נוסף אודות תביעות אסימון, ראה:

- [תביעות באסימוני גישה](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [תביעות id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [טענות](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) שאתה יכול לצפות אסימוני מזהה ואסימוני גישה שהונפקו על-ידי Azure AD B2C
- [חומר עזר לתביעות של אסימון SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
