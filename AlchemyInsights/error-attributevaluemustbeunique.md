---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813761"
---
# <a name="error-attributevaluemustbeunique"></a>שגיאה: AttributeValueMustBeUnique

הסיבה הנפוצה ביותר לשגיאה AttributeValueMustBeUnique היא שני אובייקטים בעלי SourceAnchor (immutableId) שונים בעלי ערך זהה עבור התכונות ProxyAddresses ו/או UserPrincipalName. כדי לתקן את השגיאה AttributeValueMustBeUnique:
  
1. זהה את ה- proxyAddresses, userPrincipalName או ערך תכונה אחר שגורם לשגיאה. כמו כן, זהה אילו שני אובייקטים (או יותר) מעורבים בהתנגשות. המדיניות הדוח על-ידי Azure AD Connect Health לסינכרון יכולה לעזור לך לזהות את שני האובייקטים.
    
2. זהה את האובייקט שיש להמשיך לקבל את הערך המשוכפל ולאיזה אובייקט לא אמור להיות.
    
3. הסר את הערך המשוכפל מהאובייקט שלא אמור להיות לו ערך זה. שים לב כי עליך לבצע את השינוי במדריך הכתובות ממנו המקור של האובייקט. במקרים מסוימים, ייתכן שתצטרך למחוק אחד מהאובייקטים בהתנגשות.
    
4. אם ביצעת את השינוי ב- AD המקומי, תן ל- Azure AD Connect לסנכרן את השינוי כדי לתקן את השגיאה.
    

