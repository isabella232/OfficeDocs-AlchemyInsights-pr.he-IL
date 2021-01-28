---
title: בעיות בטענות ובתכונות של אסימונים
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035892"
---
# <a name="issues-with-token-claims-and-attributes"></a>בעיות בטענות ובתכונות של אסימונים

**עדכון, קביעת תצורה או הסרה של טענות אסימון**

1. באמצעות תכלת Active Directory (תכלת לספירה), באפשרותך [להתאים אישית את סוג התביעה עבור דרישת התפקיד](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) באסימון התגובה שאתה מקבל לאחר הרשאה ליישום.
2. מפתחי יישומים יכולים להשתמש בתביעות אופציונליות ביישומי הפרסום התכולים שלהם כדי לציין אילו טענות הם מעוניינים באסימונים שנשלחו ליישום שלהם. לקבלת מידע נוסף, ראה [מתן טענות אופציונליות ליישום שלך](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [קביעת התצורה של טענות קבוצתיות עבור יישומים עם תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. אם אתה משתמש בכניסה חלקה ביישום שלך, ראה [התאמה אישית של טענות שהונפקו באסימון SAML עבור יישומים ארגוניים](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**מיפוי תכונה של תביעות**

1. כדי לקבוע את תצורת מדיניות מיפוי התביעות באמצעות PowerShell, ראה [התאמה אישית של טענות הנפלטים באסימונים עבור יישום ספציפי בדייר (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. תכונות הרחבה של סכימת מדריך הכתובות מספקות דרך לאחסון נתונים נוספים ב-תכלת Active Directory באובייקטי משתמשים ואובייקטי מדריכי כתובות אחרים, כגון קבוצות, פרטי דייר, מנהלי שירות. ניתן להשתמש רק בתכונות הרחבה באובייקטי משתמשים לצורך פליטת טענות ליישומים. [שימוש בתכונות הרחבה של סכימת מדריך הכתובות בתביעות מתאר](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) כיצד להשתמש בתכונות הרחבה של סכימת directory לשליחת נתוני משתמש ליישומים בתביעות אסימונים.

לקבלת מידע נוסף אודות טענות token, ראה:

- [טענות באסימונים של access](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [טענות בid_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [טענות](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) שניתן לצפות באסימוני מזהה ובאסימונים של access שהונפקו על-ידי תכלת AD B2C
- [הפניה לטענות של אסימון SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
