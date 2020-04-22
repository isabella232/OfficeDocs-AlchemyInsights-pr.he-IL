---
title: עבודה עם iOS VPP חוק כלל מזהה 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719958"
---
# <a name="working-with-ios-vpp-applications"></a>עבודה עם iOS VPP יישומים

קרא [כיצד לנהל את האפליקציות iOS שנרכשו באמצעות תוכנית לרכישת אמצעי אחסון עם Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות תכונות, אילוצים, ושלבים כדי לעשות שימוש בתוכנית הרכישה של אפל נפח ותמיכה עבור אותו ב-Microsoft Intune.
  
 **סוגיות נפוצות:** "הוצבתי app VPP iOS למשתמשים שלי, אבל ההתקנה נכשלה."
  
- הדבר עלול לקרות אם אסימון VPP יחיד משמש באמצעות מספר ספקי ניהול התקנים ניידים מרובים. אסימוני VPP מ-Apple יכולים לשמש רק עם ספק אחד. אם השתמשת באסימון VPP עם ספקים מרובים, עליך להעלות מחדש את האסימון ל-Intune.

- ההתקנה יכולה גם להיכשל אם המספר הכולל של ההתקנות חורג ממספר הרשיונות. כדי להציג דוח שימוש עבור הרשיונות שלך, עבור אל דף \> **היישומים Intune Mobile** **App** . כדי ללמוד כיצד להשיב רישיונות בשימוש, עיין [במאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
