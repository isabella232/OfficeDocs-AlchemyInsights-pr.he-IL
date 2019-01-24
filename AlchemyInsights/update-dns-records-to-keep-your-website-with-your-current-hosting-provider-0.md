---
title: עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472334"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>עדכון רשומות DNS כדי להשאיר את אתר האינטרנט שלך אצל ספק האירוח הנוכחי

1. בדף [תחומים](https://portal.office.com/adminportal/home#/Domains), ברשימת התחומים, בחר את התחום שבו אתה משתמש עבור אתר האינטרנט שלך ולאחר מכן בחר **הגדרות DNS** בחלונית הניהול. 
    
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
    

