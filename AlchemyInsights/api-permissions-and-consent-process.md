---
title: הרשאות API ותהליך הסכמה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404870"
---
# <a name="api-permissions-and-consent-process"></a>הרשאות API ותהליך הסכמה

כדי שהאפליקציות שלך לגשת לנתונים ב- Microsoft Graph, המשתמש או מנהל המערכת חייבים להעניק להם את ההרשאות הנכונות באמצעות תהליך הסכמה. [הפניה להרשאות Microsoft Graph מפרטת](https://docs.microsoft.com/graph/permissions-reference) את ההרשאות המשויכות לכל קבוצה ראשית של ממשקי API של Microsoft Graph. הוא מספק גם הדרכה לגבי אופן השימוש בהרשאות.

**הגדרה או עדכון של מנהל שירות**

- [יצירת serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - מאמר זה מראה לך כיצד ליצור שירות חדשאובייקטPrincipal.
- [צור יישום Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) שירות ראשי בפורטל - מאמר זה מראה לך כיצד ליצור יישום חדש של Azure Active Directory (Azure AD) ומנהל שירות, איתם ניתן להשתמש עם פקד הגישה מבוסס התפקידים.
- [אפליקציות &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) שירות ב- Azure AD - מאמר זה מתאר רישום יישומים, אובייקטי יישומים ומנהלי שירות ב- Azure Active Directory: מה הם, אופן השתמשו בהם ואופן הקשורים זה לזה.

**הוספה או עדכון של רישום אפליקציה וספק הסכמת מנהל מערכת**

- [יצירת רישום אפליקציה](https://docs.microsoft.com/graph/api/application-post-applications) - מאמר זה מראה לך כיצד ליצור אובייקט יישום חדש.
- [עדכון רישום אפליקציה - הרשאות API](https://docs.microsoft.com/graph/api/application-update) - מאמר זה מראה לך כיצד לעדכן את המאפיינים של אובייקט יישום.
- [ספק הסכמת מנהל מערכת](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - לקבלת הסכמת מנהל מערכת והסכמה באופן כללי, אנו דורשים מנהל מערכת מעניק הסכמה באופן מפורש.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - גורם מכיל לניהול תפקידים עבור הגדרות תפקיד מאוחדות והקצאות תפקיד עבור ספקי RBAC של Microsoft 365 התומכים במספר מנהלים וטווחים מרובים בהקצאת תפקיד בודדת. פעולה זו שונה מסוג *המשאב rbacApplication.* Microsoft Intune הוא דוגמה של ספק RBAC כזה. הקצאת תפקיד ב- Intune יכולה לכוללים מערך של מנהלים ומערך של קבוצות טווח. **אפשרות זו נמצאת בגירסת ביתא, כלומר שהיא עדיין בפיתוח ולא מומלצת לשימוש בייצור.**
