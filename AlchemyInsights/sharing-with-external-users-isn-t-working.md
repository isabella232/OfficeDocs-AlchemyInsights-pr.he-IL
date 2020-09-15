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
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691576"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>פתרון בעיות בשיתוף תוכן של SharePoint עם משתמשים חיצוניים

ודא ששיתוף חיצוני מופעל עבור הארגון שלך:
  
1. עבור אל [הדף תוספות שירותים &amp; במרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ולחץ על **אתרים**.
    
2. ודא שההגדרה מופעלת "On". אם האפשרות ' משתמשים חיצוניים קיימים בלבד ' נבחרה, ודא שהמשתמש החיצוני מופיע במרכז הניהול של Microsoft 365.
    
ודא ששיתוף חיצוני מופעל עבור האתר. עבור אוסף אתרים קלאסי:
  
1. במרכז הניהול החדש של SharePoint, בחלונית הימנית, לחץ על **אתרים**.
    
2. בחר את האתר או האתרים, וברצועת הכלים, לחץ על **שיתוף**.
    
עבור אתר צוות השייך לקבוצה של Microsoft 365, או לאתר תקשורת:
  
- סוגי אתרים חדשים אלה כוללים את אותה הגדרת שיתוף כהגדרה של הארגון שלך, אלא אם ההגדרה של הארגון כולה מאפשרת שיתוף קבצים באמצעות קישורים שאינם דורשים כניסה. במקרה זה, האתרים מאפשרים שיתוף עם משתמשים חיצוניים חדשים וקיימים שנכנסים. כדי לשנות את ההגדרה עבור אתרים ספציפיים, השתמש במרכז הניהול החדש של SharePoint או ב-PowerShell. [למידע נוסף](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> הגדרת השיתוף החיצוני עבור אתר כלשהו יכולה להיות מגבילה יותר מההגדרה הכלל-ארגונית שלך, אך לא יותר מאשר הגדרה של הארגון כולו. 
  

