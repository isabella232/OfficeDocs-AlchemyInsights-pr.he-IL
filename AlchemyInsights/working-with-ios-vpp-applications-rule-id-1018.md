---
title: עבודה עם iOS VPP יישומים כלל מזהה 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364853"
---
# <a name="working-with-ios-vpp-applications"></a>עבודה עם iOS יישומים VPP

קרא [כיצד לנהל יישומים iOS שנרכשו באמצעות תוכנית רכישה בכמות עם Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות התכונות, אילוצים השלבים כדי להפוך להשתמש של תוכנית רכישה של אמצעי האחסון תפוח ותמיכה עבור אותו ב- Microsoft Intune.
  
 **בעיות נפוצות:** "להקצות יישום VPP iOS המשתמשים שלי, אך ההתקנה נכשלה".
  
- הדבר יכול לקרות אם נעשה שימוש ב- token VPP יחיד על-פני מספר ספקים ניהול של מכשיר נייד. ניתן להשתמש באסימונים VPP מ- Apple רק עם ספק אחד. אם השתמשת אסימון VPP עם ספקים מרובים, עליך לטעון מחדש את האסימון כדי Intune.

- ההתקנה עלול להיכשל גם אם המספר הכולל של התקנות לחרוג ממספר הרשיונות. כדי להציג של הדוח שימוש עבור הרישיונות שלך, עבור אל **apps ניידים Intune** \> דף **רשיונות App** . כדי ללמוד כיצד לפנות רשיונות בשימוש, עיין [מאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
