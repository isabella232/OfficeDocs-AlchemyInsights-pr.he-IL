---
title: פתרון בעיות סינכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390427"
---
# <a name="troubleshoot-password-synchronization"></a>פתרון בעיות סינכרון סיסמאות

כדי לפתור בעיות שבהן הם סיסמאות לא מסונכרן עם חיבור AD תכלת הרקיע גירסה 1.1.614.0 או גירסה מתקדמת יותר:
  
1. פתח את הפעלת Windows PowerShell חדשה בשרת שלך חיבור AD תכלת הרקיע עם האפשרות **הפעל כמנהל** . 
    
2. הפעל **RemoteSigned ExecutionPolicy ערכה** או **ערכת-ExecutionPolicy בלתי מוגבלת**. 
    
3. הפעל את אשף ' התחבר AD תכלת הרקיע.
    
4. נווט * * פעילויות נוספות * * דף, בחר * * פתרון * *, ולחץ על **הבא**. 
    
5. בדף ' פתרון בעיות ', לחץ על תפריט **הפעלה כדי להפעיל את פתרון הבעיות** ב- PowerShell. 
    
6. בתפריט הראשי, בחר **לפתור בעיות סינכרון סיסמאות**. 
    
7. בתפריט המשנה, בחר **סינכרון סיסמאות אינו פועל כלל**. 
    
 **להבין את התוצאות של הפעילות לפתרון בעיות**
  
המשימה לפתרון בעיות מבצע את הבדיקות הבאות:
  
- מאמת כי תכונת הסינכרון של סיסמאות זמינה עבור דיירים תכלת הרקיע הפרסומת שלך.
    
- מאמת שרת התחבר AD תכלת הרקיע אינו נמצא במצב אחסון זמני.
    
- עבור כל קיים המקומית Active Directory מחבר (התואם יער של Active Directory קיים):
    
- 
  - מאמת את תכונת הסינכרון של סיסמאות מופעלת.
    
  - חיפוש אירועים של פעימות הסינכרון סיסמה ביומני האירועים של היישום Windows.
    
  - עבור כל תחום Active Directory תחת המחבר Active Directory מקומי:
    
  - מאמת התחום הוא אפשרות לגשת מהשרת התחבר AD תכלת הרקיע.
    
  - מאמת חשבונות ה-Active Directory Domain Services (AD DS) בשימוש על-ידי המחבר Active Directory מקומי בעל שם משתמש וסיסמה נכונים, סיסמה והרשאות הנדרש עבור סינכרון סיסמאות.
    
לקבלת עזרה נוספת לפתרון בעיות סינכרון סיסמה, ראה [פתרון בעיות סינכרון סיסמאות עם סינכרון התחבר AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

