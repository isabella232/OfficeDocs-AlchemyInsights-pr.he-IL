---
title: העברה מ- AIP ל- MIP/Unified Labeling במרכז התאימות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825372"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>העברה מ- AIP ל- MIP/Unified Labeling במרכז התאימות

כדי לעבור מתוויות AIP לתיוג מאוחד במרכז האבטחה והתאימות, עשה את הפעולות הבאות:

**הפעלת הגנה בפורטל Azure**

1. אם עדיין לא עשית זאת, פתח חלון דפדפן חדש [והירשם לפורטל Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). נווט אל **להב Azure Information Protection.** לדוגמה, בתפריט Hub, לחץ על **כל השירותים** והתחל **להקליד מידע** בתיבה מסנן. בחר **Azure Information Protection**. אם לא ניגשת ללהב Azure Information Protection בעבר, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) עיין בשלבים הנוספות ה חד-זמניים כדי להוסיף להב זה לפורטל. כדי לפתוח את להב Azure Information Protection, עליך לתכן תוכנית [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) או תוכנית Office 365 הכוללת ניהול זכויות. אם יש לך אחד מהמינויים הללו, אך אתה רואה הודעה שלא ניתן למצוא מנוי חוקי, פנה [לתמיכה של Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) או השתמש בערוצים הרגילים שלך לתמיכה.

2. אתר את **אפשרויות** התפריט ניהול ובחר הפעלת **הגנה**. לחץ **על הפעל** ולאחר מכן אשר את הפעולה. לאחר השלמת ההפעלה, סרגל המידע מציג את **ההפעלה הסתיימה בהצלחה.**

**העברת תוויות Azure Information Protection אל Office 365 Security & מרכז התאימות**

1. ודא שאתה מחובר כמשתמש בעל הרשאת מנהל מערכת כללי.

2. נווט אל **להב Azure Information Protection.**

3. מתוך אפשרות **התפריט ניהול,** בחר **אחידה תוויות**.

4. ב- **Azure Information Protection - Unified label blade,** לחץ על הפעל **ובצע** את ההוראות המקוונות.

**הערה:** ודא שיש לך את ההרשאות המתאימות לפני הפעלת העברת מרכז & האבטחה. עיין במאמרים אלה לקבלת מידע נוסף:

1. [האם עליך להיות מנהל מערכת כללי כדי לקבוע את התצורה של Azure Information Protection, או האם ניתן להקצות למנהלי מערכת אחרים?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [מידע חשוב אודות תפקידי ניהול לאחר המעבר אל מרכז האבטחה & תאימות.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

לקבלת מידע נוסף על העברת AIP להעברה אחידה של תוויות למרכז האבטחה והתאימות, ראה [העברת תוויות](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
