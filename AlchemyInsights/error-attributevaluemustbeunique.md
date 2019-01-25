---
title: שגיאה AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499635"
---
# <a name="error-attributevaluemustbeunique"></a>שגיאה: AttributeValueMustBeUnique

הסיבה הנפוצה ביותר השגיאה AttributeValueMustBeUnique היא שני אובייקטים עם SourceAnchor שונים (immutableId) בעלי אותו ערך עבור התכונות ProxyAddresses ו/או UserPrincipalName. כדי לתקן את השגיאה AttributeValueMustBeUnique:
  
1. זהה proxyAddresses כפול, userPrincipalName או אחרים עבור ערך התכונה גורם לשגיאה. גם לזהות אילו אובייקטים פעמיים (או יותר) מעורבים בהתנגשות. הדוח שנוצר על-ידי תקינות להתחבר AD של תכלת הרקיע עבור סינכרון יכול לסייע לך לזהות את שני האובייקטים.
    
2. לזהות איזה אובייקט עליך להמשיך לקיים את הערך המשוכפלת ואת איזה אובייקט אינו אמור להכיל.
    
3. להסיר את הערך המשוכפלת האובייקט לא יכולים להיות ערך זה. שים לב כי יש לבצע את השינוי בספריה שבה האובייקט sourced מתוך. במקרים מסוימים, ייתכן שיהיה עליך למחוק אחד האובייקטים מתנגשים.
    
4. אם ביצעת את השינוי בהמקומית על הפרסומת, מאפשרים חיבור AD תכלת הרקיע לסנכרן את השינוי עבור השגיאה לקבל קבוע.
    

