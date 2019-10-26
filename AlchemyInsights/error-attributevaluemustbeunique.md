---
title: שגיאה בייחוס מיוחד
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
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36526998"
---
# <a name="error-attributevaluemustbeunique"></a>שגיאה: ייחס ערך מיוחד

הסיבה השכיחה ביותר לשגיאות הייחודיות היא שני אובייקטים עם נקודת מקור שונה (immutableId) בעלי ערך זהה עבור התכונות של כתובות ProxyAddresses/או מאפייני שם המשתמש. כדי לתקן את השגיאה הייחודית:
  
1. זהה את הכתובות המשוכפלת של proxyAddresses, או ערך תכונה אחר שגורם לשגיאה. כמו כן, זהה אילו שני אובייקטים (או יותר) מעורבים בהתנגשות. הדו ח שנוצר על ידי תכלת AD התחברות בריאות לסנכרון יכול לעזור לך לזהות את שני האובייקטים.
    
2. זהה את האובייקט שעליו להמשיך להיות בעל הערך המשוכפל והאובייקט שאין להוסיף לו.
    
3. הסר את הערך המשוכפל מהאובייקט שאינו אמור להיות בעל ערך זה. שים לב שעליך לבצע את השינוי בספריה ממנו מקור האובייקט. במקרים מסוימים, ייתכן שיהיה עליך למחוק אחד מהאובייקטים בהתנגשות.
    
4. אם ביצעת את השינוי ב-AD המקומי, הנח לתכלת החיבור לסנכרן את השינוי כדי שהשגיאה תהיה קבועה.
    

