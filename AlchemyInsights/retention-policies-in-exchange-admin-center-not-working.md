---
title: מדיניות שמירה במרכז הניהול של Exchange אינה פועלת
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952229"
---
# <a name="retention-policies-in-exchange-admin-center"></a>מדיניות שמירה במרכז הניהול של Exchange

אם ברצונך שנריץ בדיקות אוטומטיות עבור ההגדרות שהוזכרו להלן, בחר את לחצן הקודם <- בחלק העליון של דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שיש לו בעיות במדיניות שמירה.

אם אתה נתקל בבעיות במדיניות שמירה במרכז הניהול של Exchange שלא חלות על תיבות דואר או על פריטים שלא עוברים לתיבת הדואר של הארכיון, בדוק את הפעולות הבאות:

**סיבות בסיס:**

- **מסייע התיקיות** המנוהלים לא עיבד את תיבת הדואר של המשתמש. מסייע התיקיות המנוהלים מנסה לעבד כל תיבת דואר בארגון המבוסס על ענן צמתים פעם בשבעה ימים.

  **הפתרון:** הפעל את מסייע התיקיות המנוהלים.

- **RetentionHold** הופעל **בתיבת** הדואר. אם תיבת הדואר ממוקמת ב- RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה.

  **הפתרון:** בדוק את המצב של הגדרת החזקת שמירה ועדכן אותו כצורך. לקבלת פרטים, ראה [החזקת שמירת תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**הערה:** אם תיבת דואר קטנה מ- 10 MB, מסייע התיקיות המנוהלים לא יעבד באופן אוטומטי את תיבת הדואר.
 
לקבלת מידע נוסף על מדיניות שמירה במרכז הניהול של Exchange, ראה:

- [תגיות שמירה ומדיניות שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [החלת מדיניות שמירה על תיבות דואר או](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [הוספה או הסרה של תגיות שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [כיצד לזהות את סוג הה להחזיק בתיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
