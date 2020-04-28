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
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913003"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>תיקון בעיות בשיתוף תוכן SharePoint עם משתמשים חיצוניים

ודא ששיתוף חיצוני מופעל עבור הארגון שלך:
  
1. עבור אל [דף התוספות של &amp; שירותים במרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ולחץ על **אתרים**.
    
2. ודא שההגדרה הפכה ל-"On". אם נבחר "רק משתמשים חיצוניים קיימים", ודא שהמשתמש החיצוני מופיע במרכז הניהול של Microsoft 365.
    
ודא ששיתוף חיצוני מופעל עבור האתר. לקבלת אוסף אתרים קלאסי:
  
1. במרכז הניהול החדש של SharePoint, בחלונית הימנית, לחץ על **אתרים**.
    
2. בחר את האתר או האתרים, וברצועת הכלים, לחץ על **שיתוף**.
    
עבור אתר צוות השייך לקבוצת Microsoft 365 או לאתר תקשורת:
  
- לסוגי אתרים חדשים אלה יש הגדרת שיתוף זהה לזו של הגדרת הארגון שלך, אלא אם כן ההגדרה כלל-ארגונית מאפשרת שיתוף קבצים באמצעות קישורים שאינם דורשים כניסה. במקרה זה, האתרים מאפשרים שיתוף עם משתמשים חיצוניים חדשים וקיימים החותמים. כדי לשנות את ההגדרה עבור אתרים מסוימים, השתמש במרכז הניהול החדש של SharePoint או ב-PowerShell. [למידע נוסף](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> הגדרת השיתוף החיצוני עבור כל אתר יכולה להיות מגבילה יותר מההגדרה הכלל-ארגונית, אך לא יותר מתירני מאשר ההגדרה הכלל-ארגונית. 
  

