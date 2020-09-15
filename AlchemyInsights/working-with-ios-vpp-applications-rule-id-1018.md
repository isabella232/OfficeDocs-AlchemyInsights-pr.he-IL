---
title: עבודה עם iOS VPP Applications Rule Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688947"
---
# <a name="working-with-ios-vpp-applications"></a>עבודה עם יישומים של iOS VPP

קרא [כיצד לנהל יישומי iOS שנרכשו באמצעות תוכנית לרכישת נפח עם Microsoft intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות תכונות, אילוצים ושלבים לביצוע השימוש בתוכנית לרכישת נפח של Apple והתמיכה בה ב-Microsoft intune.
  
 **בעיות נפוצות:** "הוצבתי אפליקציית iOS VPP למשתמשים שלי, אך ההתקנה נכשלה."
  
- פעולה זו עשויה להתרחש אם אסימון אחד של VPP נמצא בשימוש בין ספקי ניהול מכשירים ניידים מרובים. ניתן להשתמש באסימונים של VPP מ-Apple רק עם ספק אחד. אם השתמשת באסימון VPP עם ספקים מרובים, עליך להעלות מחדש את האסימון לכיוון המנגינה.

- ההתקנה יכולה גם להיכשל אם מספר ההתקנות הכולל חורג ממספר הרשיונות. כדי להציג דוח שימוש עבור הרשיונות שלך, עבור לדף רשיונות האפליקציה ' **כוונון אפליקציות למכשירים ניידים** ' \> **App licenses** . כדי ללמוד כיצד להחזיר רשיונות בשימוש, עיין [במאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
