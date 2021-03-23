---
title: קביעת התצורה של נקודת חיבור שירות (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036142"
---
# <a name="configure-service-connection-point-scp"></a>קביעת התצורה של נקודת חיבור שירות (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **סיבה**: אין אפשרות לקרוא את האובייקט SCP ולקבל את המידע על הדייר של תכלת לספירה
- **פתרון**: עיין בסעיף [קביעת תצורה של נקודת חיבור לשירות](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**תוכנית פעולה**

- בדוק אם המכשיר קיבל את ה-GPO עבור האימות המבוקר.
- ודא ש-GPO יצר את מפתחות הרישום.
- ודא שיש לך שני מקשים שנוצרו באמצעות מזהה הספריה והתחום של onmicrosoft.

**קביעת התצורה של הגדרת רישום בצד הלקוח עבור SCP**

השתמש בדוגמה הבאה כדי ליצור אובייקט מדיניות קבוצתית (GPO) כדי לפרוס הגדרת רישום הקובעת ערך SCP ברישום של המכשירים שלך.

1. פתח מסוף ניהול מדיניות קבוצתית וצור GPO חדש בתחום שלך.
     - ספק שם לאובייקט ה-GPO החדש שיצרת (לדוגמה, ClientSideSCP)

2. ערוך את ה-GPO ואתר את הנתיב הבא: **תצורת מחשב > העדפות > הגדרות Windows > רישום**.

3. לחץ באמצעות לחצן העכבר הימני על **הרישום** ובחר **פריט רישום חדש >**.

4. בכרטיסיה **כללי** , קבע את תצורת הפעולות הבאות:
  
- **פעולה**: עדכון
    
- **כוורת**: HKEY_LOCAL_MACHINE
    
- **נתיב מפתח**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **שם ערך**: TenantId
    
- **סוג ערך**: REG_SZ
    
- **נתוני ערך**: GUID או מזהה מדריך הכתובות של מופע ה-"תכלת לספירה" (ערך זה ניתן למצוא **בפורטל תכלת > תכלת active Directory > מאפיינים > מזהה מדריך כתובות**)
 
- לחץ על **אישור**.
 
5. לחץ באמצעות לחצן העכבר הימני על **הרישום** ובחר **פריט רישום חדש >**.

6. בכרטיסיה **כללי** , קבע את תצורת הפעולות הבאות:
  
- **פעולה**: עדכון
    
- **כוורת**: HKEY_LOCAL_MACHINE
    
- **נתיב מפתח**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **שם ערך**: TenantName
    
- **סוג ערך**: REG_SZ
    
- **נתוני ערך**: שם התחום המאומת שלך אם אתה משתמש בסביבה מאוחדת כגון AD FS. שם התחום שאומת או שם התחום שלך ב-onmicrosoft.com (לדוגמה, contoso. onmicrosoft). com אם אתה משתמש בסביבה מנוהלת

- לחץ על **אישור**.

7. סגור את העורך עבור ה-GPO החדש שנוצר.

8. קשר את ה-GPO החדש שנוצר לקבוצה הרצויה של OU המכילה מחשבים המצורפים לתחום השייכים לאוכלוסיית הפריסה הנשלטת.

לקבלת מידע נוסף, ראה [אימות מבוקר של הצטרפות כלאיים של תכלת-תכלת לספירה | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [ופתרון בעיות היברידית תכלת active Directory הצטרפו למכשירים | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









