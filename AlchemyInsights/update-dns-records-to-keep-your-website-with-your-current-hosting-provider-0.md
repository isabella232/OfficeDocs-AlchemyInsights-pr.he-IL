---
title: עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007683"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי

1. בתיבת מרכז הניהול של Microsoft 365, עבור אל הדף **הגדרת**  >  [תחומים,](https://admin.microsoft.com/Adminportal#/Domains) וברשימת התחומים, בחר את התחום שאתה משתמש בו עבור אתר האינטרנט שלך.

2. בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:

  - עבור **סוג DNS** הזן: **A (כתובת)**

  - עבור **שם מארח או כינוי**, הקלד: **@**

  - עבור **כתובת IP**, הקלד את כתובת ה- IP הסטטית עבור אתר האינטרנט שלך במקום שבו הוא מתארח כעת (לדוגמה, 172.16.140.1‏).

    כתובת זו חייבת להיות כתובת IP  *סטטית*  עבור אתר האינטרנט, ולא כתובת IP  *דינאמית*  . בדוק באתר שבו מתארח אתר האינטרנט שלך כדי לוודא שבאפשרותך לקבל כתובת IP סטטית עבור אתר האינטרנט הציבורי.

3. בחר **שמור**.

ניתן גם ליצור רשומת CNAME כדי לעזור למבקרים למצוא את אתר האינטרנט שלך.
  
1. בחר **+ רשומה מותאמת אישית חדשה** והזן את הפרטים הבאים:

  - עבור **סוג DNS** הזן: **CNAME (כינוי)‎**

  - עבור **שם מארח או כינוי**, הקלד: **www**

  - עבור **כתובת מפנה**, הקלד את שם התחום המלא (FQDN) של אתר האינטרנט שלך (לדוגמה, contoso.com).

2. בחר **שמור**.
