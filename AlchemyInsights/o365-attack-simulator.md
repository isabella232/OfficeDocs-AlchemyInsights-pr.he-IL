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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801552"
---
# <a name="attack-simulator-in-microsoft-365"></a>סימולטור התקפה ב-Microsoft 365

- האם חסר לך סימולטור התקפה? סימולטור **התקפה דורש Microsoft Defender עבור office 365 תוכנית 2 (ATP תוכנית 2)** או **Office 365 Enterprise E5** . סימולטור התקפה **אינו** כלול ב-Microsoft Defender עבור Office 365 תוכנית 1 (ATP Plan 1), Office 365 Enterprise E3, או כל אפליקציות Microsoft 365 למנויים עסקיים.

- החשבון שבו אתה משתמש להפעלת התקפות מדומה דורש הרשאות מנהל מערכת כללי או מנהל אבטחה ואימות רב-גורמי. לקבלת מידע נוסף אודות דרישות סימולטור התקפה, עיין [בנושא זה](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- דברים חשובים שעליך לדעת על סימולציות התקפה **בסיסמאות של כוח פיזי** :

  - אם חשבון היעד הזמין את משרד המשתמש והסיסמה התמלאה כראוי, החשבון לא יוצג כסכנה (מקדם האימות השני לא יהיה שלם).

  - קובץ הסיסמה אינו יכול להיות גדול מ-10 MB. השתמש בסיסמה אחת בכל שורה וכלול שורה ריקה (החזרת גררה) לאחר הסיסמה האחרונה ברשימה.

- דברים חשובים שעליך לדעת לגבי הדמיית **החנית** מצרף סימולציות:

  - לפי עיצוב, אין באפשרותך לספק ערך מותאם אישית עבור **כתובת URL של שרת הכניסה לדיוג** .

  - אם נמען משתמש [בתוספת הפיכת הודעת הדוח לזמינה](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) כדי לדווח על ההודעה כדיוג, ייתכן שלא תקבל התראות עבור ההודעה (מכיוון שזוהי התקפה מדומה).

- דוחות: לאחר השלמת ההתקפה המדומה, באפשרותך ללחוץ על **פרטי התקפה** כדי לראות את הדוח.

- לקבלת הוראות מפורטות ותכונות חדשות בסימולטור התקפה, ראה [סימולטור התקפה ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
