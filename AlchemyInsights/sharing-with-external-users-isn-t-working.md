---
title: שיתוף עם משתמשים חיצוניים אינו פועל
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767250"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>תיקון בעיות בשיתוף תוכן SharePoint עם משתמשים חיצוניים

ודא ששיתוף חיצוני מופעל עבור הארגון שלך:
  
1. עבור אל [דף התוספות של &amp; שירותים במרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ולחץ על **אתרים**.
    
2. ודא שההגדרה הפכה ל-"On". אם נבחר "רק משתמשים חיצוניים קיימים", ודא שהמשתמש החיצוני מופיע במרכז הניהול של Microsoft 365.
    
ודא ששיתוף חיצוני מופעל עבור האתר. לקבלת אוסף אתרים קלאסי:
  
1. במרכז הניהול החדש של SharePoint, בחלונית הימנית, לחץ על **אתרים**.
    
2. בחר את האתר או האתרים, וברצועת הכלים, לחץ על **שיתוף**.
    
עבור אתר צוות השייך לקבוצת Office 365 או לאתר תקשורת:
  
- לסוגי אתרים חדשים אלה יש הגדרת שיתוף זהה לזו של הגדרת הארגון שלך, אלא אם כן ההגדרה כלל-ארגונית מאפשרת שיתוף קבצים באמצעות קישורים שאינם דורשים כניסה. במקרה זה, האתרים מאפשרים שיתוף עם משתמשים חיצוניים חדשים וקיימים החותמים. כדי לשנות את ההגדרה עבור אתרים מסוימים, השתמש במרכז הניהול החדש של SharePoint או ב-PowerShell. [למידע נוסף](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> הגדרת השיתוף החיצוני עבור כל אתר יכולה להיות מגבילה יותר מההגדרה הכלל-ארגונית, אך לא יותר מתירני מאשר ההגדרה הכלל-ארגונית. 
  

