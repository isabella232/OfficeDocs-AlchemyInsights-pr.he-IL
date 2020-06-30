---
title: גישה מותנית עם Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931432"
---
# <a name="conditional-access-with-intune"></a>גישה מותנית עם Intune

שימוש **בגישה מותנית** עם Intune דורש 3 שלבים:

- צור **מדיניות תאימות** ([דמוי אדם](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) כדי להגדיר הגדרות שחייבות להיות מולאו לפני שההתקן נחשב לתואם. לדוגמה, על התקן להיות בעל pin של 6 ספרות לפחות לפני שהוא נחשב לתואם.
- צור **מדיניות גישה מותנית** המגדירה אילו משאבים מוגנים ואילו תנאים יש להכיר כדי לגשת למשאבים אלה.  [לדוגמה,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) על התקן להיות תואם לפני הגישה לדואר אלקטרוני של חברה.
- ודא **שמדיניות התאימות** **ופריטי מדיניות הגישה המותנים** מיועדים לקבוצות המשתמשים הרצויות. הדבר עשוי לדרוש יצירת קבוצות מסוימות של משתמשים בספריית הפעילות התכלת.

**קישורים מועילים:**

[סקירת תאימות התקנים](https://docs.microsoft.com/intune/device-compliance-get-started)

[פתרון בעיות של CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[מדיניות פתרון בעיות](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

כדי להגן על דואר אלקטרוני (Exchange online) מפני גישה על-ידי התקנים שאינם תואמים, יש לעקוב אחר שני המסמכים:

1. [הגן על גישה לדואר אלקטרוני ממכשירים באמצעות המלווים](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [הגן על גישה לדואר אלקטרוני ממכשירים באמצעות לקוחות אימות מודרניים כמו Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)