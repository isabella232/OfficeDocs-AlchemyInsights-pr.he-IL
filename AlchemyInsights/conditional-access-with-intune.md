---
title: מותן Access Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069713"
---
# <a name="conditional-access-with-intune"></a>מותן Access Intune

שימוש  **ב- Access עם**  Intune דורש 3 שלבים:

- צור מדיניות **תאימות** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) כדי להגדיר הגדרות שיש לבצע לפני שהמכשיר ייחשב לתואם. לדוגמה, למכשיר חייב להיות מספר זיהוי של לפחות 6 ספרות לפני שהוא נחשב לתואם.
- צור מדיניות **Access מותנות**  שמגדירה אילו משאבים מוגנים, ואל אילו תנאים יש לגשת למשאבים אלה.  [לדוגמה,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  מכשיר חייב להיות תואם לפני גישה לדואר אלקטרוני ארגוני.
- ודא **שמדיניות תאימות ומדיניות**  **Access מותנה**  ממוקדים לקבוצות המשתמשים הרצויות. פעולה זו עשויה לדרוש יצירת קבוצות ספציפיות של משתמשים ב- Azure Active Directory.

**קישורים שימושיים:**

[מבט כולל על תאימות מכשירים](https://docs.microsoft.com/intune/device-compliance-get-started)

[פתרון בעיות ב- CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[מדיניות פתרון בעיות](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

כדי להגן על דואר אלקטרוני (Exchange באינטרנט) מפני גישה על-ידי מכשירים שאינם תואמים, יש לעקוב אחר שני המסמכים:

1. [הגן על הגישה לדואר אלקטרוני ממכשירים באמצעות EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [הגן על גישת דואר אלקטרוני ממכשירים באמצעות לקוחות אימות מודרניים, כגון Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)