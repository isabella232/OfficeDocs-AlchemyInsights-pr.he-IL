---
title: שיתוף עם משתמשים חיצוניים אינו פועל
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502232"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>פתור בעיות שיתוף תוכן SharePoint עם משתמשים חיצוניים

ודא כי שיתוף חיצוני מופעלת עבור הארגון שלך:
  
1. עבור אל [שירותי &amp; דף תוספות במרכז admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), לחץ על **אתרים**.
    
2. ודא כי ההגדרה מופעלת כדי "On". אם נבחר "רק קיימים משתמשים חיצוניים", ודא שמופיע משתמש חיצוני במרכז הניהול של Microsoft 365.
    
ודא חיצוני שיתופו מופעלת עבור האתר. עבור אוסף אתרים קלאסי:
  
1. במרכז הניהול של SharePoint חדש, בחלונית הימנית, לחץ על **אתרים**.
    
2. בחר אתר או אתרים ולאחר ברצועת הכלים, לחץ על **שיתוף**.
    
עבור אתר של צוות השייך לקבוצת Office 365, או אתר תקשורת:
  
- סוגים אלה של האתר החדש יש את אותו שיתוף הגדרת כהגדרה ברחבי הארגון שלך, אלא אם כן הגדרת ארגוני מאפשרת שיתוף קבצים באמצעות קישורים שאינן דורשות הכניסה. במקרה זה, האתרים אפשר שיתוף עם משתמשים חיצוניים חדשים וקיימים להיכנס. כדי לשנות את ההגדרה עבור אתרים מסוימים, השתמש מרכז הניהול החדש של SharePoint או PowerShell. [פרטים נוספים](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> ההגדרה שיתוף חיצוני עבור כל אתר יכול להיות מגבילות יותר את הגדרת הארגון כולו, אך ולקוד לא יותר מההגדרה של הארגון כולו. 
  

