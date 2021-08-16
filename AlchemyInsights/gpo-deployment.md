---
title: פריסת GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067841"
---
# <a name="gpo-deployment"></a>פריסת GPO

הגדרות עבור אובייקטי משתמש ומחשב ב- Azure Active Directory Domain Services (Azure AD DS) מנוהלים לעתים קרובות באמצעות אובייקטי מדיניות קבוצתית (GPO). Azure AD DS כולל אובייקטי GPO מוכללים עבור גורמים מכילים של משתמשי AADDC ומחשבים של AADDC. באפשרותך להתאים אישית אובייקטי GPO מוכללים אלה כדי לקבוע את התצורה של מדיניות קבוצתית לפי הצורך עבור הסביבה שלך. לחברים בקבוצה מנהלי מערכת של Azure AD DC יש הרשאות ניהול מדיניות קבוצתית בתחום Azure AD DS, והם יכולים גם ליצור אובייקטי GPO מותאמים אישית ויחידות ארגוניות (OUs). לקבלת מידע נוסף אודות מדיניות קבוצתית ואופן העבודות שלה, ראה מבט כולל [על מדיניות קבוצתית](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

בסביבה היברידית, פריטי מדיניות קבוצתית המוגדרים בסביבה מקומית של AD DS אינם מסונכרנים עם Azure AD DS. כדי להגדיר הגדרות תצורה עבור משתמשים או מחשבים ב- Azure AD DS, ערוך אחד מ- GPO המוגדרים כברירת מחדל או צור GPO מותאם אישית.

מאמר זה [ניהול מדיניות קבוצתית](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) מראה לך כיצד להתקין את כלי ניהול המדיניות הקבוצתית, כיצד לערוך את אובייקטי ה- GPO המוכללים ואופן יצירת אובייקטי GPO מותאמים אישית.
