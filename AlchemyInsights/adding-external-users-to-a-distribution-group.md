---
title: הוספת משתמשים חיצוניים לקבוצת תפוצה
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934834"
---
# <a name="add-external-users-to-a-distribution-group"></a>הוספת משתמשים חיצוניים לקבוצת תפוצה

הוספת איש קשר חיצוני לקבוצת תפוצה (DG) היא תהליך דו-שליט:
  
1. צור איש קשר של דואר עבור המשתמש החיצוני:
    
    1. במרכז הניהול, עבור אל הדף **אנשי**  >  [קשר של](https://admin.microsoft.com/adminportal/home#/Contact) משתמשים. 
    
    2. בחר **הוסף איש קשר**.
    
    3. הקלד את המידע עבור איש הקשר שלך ובחר **הוסף**.
    
2. הוסף את איש הקשר של הדואר ל- DG:
    
    1. במרכז הניהול, עבור אל הדף  >  [קבוצות](https://admin.microsoft.com/adminportal/home#/groups) קבוצות. 
    
    2. אתר את ה- DG שברצונך להוסיף לו את המשתמש החיצוני ובחר אותו כדי לפתוח את תיבת הדו-שיח לעריכה.
    
    3. בכרטיסיה **חברים,** בחר הצג **את כל החברים ונהל אותם.** 
    
    4. בחר **הוסף חברים**.
    
    5. בחר את איש הקשר של הדואר שיצרת בשלב הקודם ולאחר מכן בחר **שמור**.
    
אם לאחר ביצוע שלבים אלה המשתמשים החיצוניים שלך אינם יכולים לשלוח הודעות דואר אלקטרוני ל- DG או לא לקבל ממנו הודעות דואר אלקטרוני, ייתכן שה- DG מסומן לאפשר רק הודעות דואר אלקטרוני ממשתמשים פנימיים. באפשרותך לבדוק תצורה זו ולתקן אותה לאחר ההוראות [כאן.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **הערה:** הוראות אלה לא חלות אם סוג הקבוצה שלך הוא "Microsoft 365" במקום "קבוצת תפוצה". במקרה זה, באפשרותך להוסיף את המשתמש החיצוני ישירות לקבוצה מתוך Outlook. במאמר זה ניתן למצוא מידע מפורט Microsoft 365 קבוצות קבוצות, וכן הוראות להוספת אורחים [חיצוניים.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  