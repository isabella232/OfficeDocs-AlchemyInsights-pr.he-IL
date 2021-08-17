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
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083015"
---
# <a name="working-with-ios-vpp-applications"></a>עבודה עם יישומי vPP של iOS

קרא כיצד לנהל יישומי iOS שנרכשו באמצעות [תוכנית רכישה רבת משתמשים עם Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות תכונות, אילוצים ושלבים כדי להשתמש בתוכנית הרכישה של נפח האחסון של Apple והתמיכה עבורה Microsoft Intune.
  
 **בעיות נפוצות:** "הקציתי יישום iOS VPP למשתמשים שלי, אך ההתקנה נכשלה".
  
- מצב זה עשוי להתרחש אם נעשה שימוש באסימון VPP יחיד בכל ספקי ניהול מכשירים ניידים מרובים. ניתן להשתמש באסימוני VPP מ- Apple רק עם ספק אחד. אם השתמשת באסימון VPP עם ספקים מרובים, עליך להעלות מחדש את האסימון ל- Intune.

- ההתקנה עשויה להיכשל גם אם המספר הכולל של התקנות חורג ממספר הרשיונות. כדי להציג שימוש הדוח עבור הרשיונות שלך, עבור אל הדף **רשיונות יישומים של יישומי Intune** \> **Mobile.** כדי ללמוד כיצד לקבל מחדש רשיונות בשימוש, עיין [במאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
