---
title: שגיאה AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709152"
---
# <a name="error-attributevaluemustbeunique"></a>שגיאה: AttributeValueMustBeUnique

הסיבה הנפוצה ביותר לשגיאה AttributeValueMustBeUnique היא שני אובייקטים עם SourceAnchor שונים (immutableId), שאותו ערך עבור התכונות ProxyAddresses ו/או UserPrincipalName. כדי לתקן את השגיאה AttributeValueMustBeUnique:
  
1. זהה את הערך המשוכפל proxyAddresses, userPrincipalName או ערך תכונה אחר שגורם לשגיאה. זהה גם אילו שני (או יותר) אובייקטים מעורבים בהתנגשות. הדוח שנוצר על-ידי מרכז הבריאות ' חבר בריאות לסינכרון ' יכול לעזור לך לזהות את שני האובייקטים.
    
2. זיהוי האובייקט שאמור להמשיך להיות בעל הערך המשוכפל והאובייקט שאינו אמור להימשך.
    
3. הסר את הערך המשוכפל מהאובייקט שאמור לכלול ערך זה. שים לב שעליך לערוך את השינוי במדריך הכתובות שממנו מקור האובייקט. במקרים מסוימים, ייתכן שיהיה עליך למחוק אחד מהאובייקטים המתנגשים.
    
4. אם ביצעת את השינוי בהודעה מקומית, תן ל-"תכלת AD Connect" לסנכרן את השינוי עבור השגיאה כדי להיפתר.
    

