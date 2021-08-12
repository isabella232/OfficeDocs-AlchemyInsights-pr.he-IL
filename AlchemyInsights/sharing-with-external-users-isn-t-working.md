---
title: שיתוף עם משתמשים חיצוניים אינו פועל
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910367"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>פתרון בעיות בשיתוף SharePoint תוכן עם משתמשים חיצוניים

ודא שהשיתוף החיצוני מופעל עבור הארגון שלך:
  
1. עבור אל [הדף תוספות שירותים &amp; בתיבת מרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ולאחר מכן לחץ על **אתרים**.
    
2. ודא שההגדרה מופעלת ל-"מופעל". אם האפשרות "משתמשים חיצוניים קיימים בלבד" נבחרה, ודא שהמשתמש החיצוני מופיע ברשימה מרכז הניהול של Microsoft 365.
    
ודא שהשיתוף החיצוני מופעל עבור האתר. עבור אוסף אתרים קלאסי:
  
1. במרכז הניהול SharePoint, בחלונית הימנית, לחץ על **אתרים**.
    
2. בחר את האתר או האתרים וברצועת הכלים, לחץ על **שיתוף**.
    
עבור אתר צוות השייך לקבוצת Microsoft 365 או לאתר תקשורת:
  
- סוגי אתרים חדשים אלה עשויים להיות זהים להגדרת השיתוף של ההגדרה של הארגון כולו, אלא אם כן ההגדרה ברחבי הארגון מאפשרת שיתוף קבצים באמצעות קישורים שלא דורשים כניסה. במקרה זה, האתרים מאפשרים שיתוף עם משתמשים חיצוניים חדשים וקיימים שהכניסה. כדי לשנות את ההגדרה עבור אתרים ספציפיים, השתמש במרכז הניהול SharePoint או ב- PowerShell. [למידע נוסף](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> הגדרת השיתוף החיצוני עבור כל אתר יכולה להיות מגבילה יותר מההגדרה של הארגון כולו, אך אינה מתירת יותר מההגדרה של הארגון כולו. 
  

