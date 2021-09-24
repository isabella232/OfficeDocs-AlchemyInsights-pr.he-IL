---
title: הוספת תחום משנה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506487"
---
# <a name="adding-a-sub-domain"></a>הוספת תחום משנה

ניתן להוסיף תחומי משנה לאותו דייר או לדייר אחר מאשר בתחום האב. בכל מקרה, עליך לנהל הגדרות DNS משלך באתר האינטרנט של הרשם שלך. אם נתת ל- Microsoft לנהל את הגדרות ה- DNS שלך באמצעות רשומות NS, או אם קנית את התחום מ- Microsoft, לא ניתן להוסיף תחומי משנה מבלי לשנות זאת תחילה.

הוסף תחילה את תחום האב ולאחר מכן הוסף את תחום המשנה. אם תחום המשנה נמצא באותו דייר, לא נדרש אימות נוסף. אם תוסיף את תחום המשנה לדייר נפרד, רשומת ה- DNS txt נדרשת לאימות בעלות לפני הוספת התחום והרשומות הנוספות של ה- DNS עבור השירותים שנבחרו.

- כדי להוסיף תחום או תחום משנה, בצע את אשף [הוספת תחום](https://admin.microsoft.com/Adminportal#/Domains/Wizard)או הוסף את התחום או תחום המשנה באופן ידני על-ידי מעבר אל **הגדרת**  >    >  **תחומים הוסף תחום**.

אם יש צורך בכך:

- כדי לשנות מי מנהל את הגדרות ה- DNS שלך עבור תחום קיים, **עבור אל הגדרות**  >  [**תחומים**](https://admin.microsoft.com/Adminportal/Home#/Domains), בחר את תיבת הסימון לצד התחום ולאחר מכן בחר ניהול **DNS**. באשף, בחר הוסף **רשומות DNS משלך והשלם** את האשף.
- כדי להוסיף תחומי משנה לתחום שנרכש על-ידי Microsoft, העבר תחילה את התחום לרשם אחר ולאחר מכן בצע את השינוי לעיל כדי לנהל רשומות DNS משלך. לקבלת הוראות, [ראה העברת תחום מ- Microsoft למארח אחר.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- אם אתה מקבל שגיאה שהתחום שלך כבר נמצא בשימוש על-ידי חברים או אנשים אחרים בארגון שלך, תחילה עליך לקחת על תחילה חשבון לא מנוהל זה לפני השימוש בתחום. לקבלת הוראות, ראה [ניהול מדריך כתובות לא מנוהל כמנהל מערכת ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
