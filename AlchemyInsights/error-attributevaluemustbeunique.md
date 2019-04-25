---
title: שגיאה AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402704"
---
# <a name="error-attributevaluemustbeunique"></a>שגיאה: AttributeValueMustBeUnique

הסיבה הנפוצה ביותר השגיאה AttributeValueMustBeUnique היא שני אובייקטים עם SourceAnchor שונים (immutableId) בעלי אותו ערך עבור התכונות ProxyAddresses ו/או UserPrincipalName. כדי לתקן את השגיאה AttributeValueMustBeUnique:
  
1. זהה proxyAddresses כפול, userPrincipalName או אחרים עבור ערך התכונה גורם לשגיאה. גם לזהות אילו אובייקטים פעמיים (או יותר) מעורבים בהתנגשות. הדוח שנוצר על-ידי תקינות להתחבר AD של תכלת הרקיע עבור סינכרון יכול לסייע לך לזהות את שני האובייקטים.
    
2. לזהות איזה אובייקט עליך להמשיך לקיים את הערך המשוכפלת ואת איזה אובייקט אינו אמור להכיל.
    
3. להסיר את הערך המשוכפלת האובייקט לא יכולים להיות ערך זה. שים לב כי יש לבצע את השינוי בספריה שבה האובייקט sourced מתוך. במקרים מסוימים, ייתכן שיהיה עליך למחוק אחד האובייקטים מתנגשים.
    
4. אם ביצעת את השינוי בהמקומית על הפרסומת, מאפשרים חיבור AD תכלת הרקיע לסנכרן את השינוי עבור השגיאה לקבל קבוע.
    

