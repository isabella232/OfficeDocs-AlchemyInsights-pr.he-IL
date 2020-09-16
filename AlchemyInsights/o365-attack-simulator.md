---
title: סימולטור התקפה של 2681 ב-Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759220"
---
# <a name="attack-simulator-in-microsoft-365"></a>סימולטור התקפה ב-Microsoft 365

- האם חסר לך סימולטור התקפה? סימולטור **התקפה דורש office 365 הגנה מתקדמת תוכנית הגנה 2 (ATP תוכנית 2)** או **Office 365 Enterprise E5**. סימולטור התקפה **אינו** כלול ב-Office 365 הגנה מתקדמת של תוכנית 1 (ATP plan 1), Office 365 Enterprise E3 או כל אפליקציות של Microsoft 365 למנויים עסקיים.

- החשבון שבו אתה משתמש להפעלת התקפות מדומה דורש הרשאות מנהל מערכת כללי או מנהל אבטחה ואימות רב-גורמי. לקבלת מידע נוסף אודות דרישות סימולטור התקפה, עיין [בנושא זה](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- דברים חשובים שעליך לדעת על סימולציות התקפה **בסיסמאות של כוח פיזי** :

  - אם חשבון היעד הזמין את משרד המשתמש והסיסמה התמלאה כראוי, החשבון לא יוצג כסכנה (מקדם האימות השני לא יהיה שלם).

  - קובץ הסיסמה אינו יכול להיות גדול מ-10 MB. השתמש בסיסמה אחת בכל שורה וכלול שורה ריקה (החזרת גררה) לאחר הסיסמה האחרונה ברשימה.

- דברים חשובים שעליך לדעת לגבי הדמיית **החנית** מצרף סימולציות:

  - לפי עיצוב, אין באפשרותך לספק ערך מותאם אישית עבור **כתובת URL של שרת הכניסה לדיוג**.

  - אם נמען משתמש [בתוספת הפיכת הודעת הדוח לזמינה](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) כדי לדווח על ההודעה כדיוג, ייתכן שלא תקבל התראות עבור ההודעה (מכיוון שזוהי התקפה מדומה).

- דוחות: לאחר השלמת ההתקפה המדומה, באפשרותך ללחוץ על **פרטי התקפה** כדי לראות את הדוח.

- לקבלת הוראות מפורטות ותכונות חדשות בסימולטור התקפה, ראה [סימולטור התקפה ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
