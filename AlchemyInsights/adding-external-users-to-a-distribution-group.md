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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663514"
---
# <a name="add-external-users-to-a-distribution-group"></a>הוספת משתמשים חיצוניים לקבוצת תפוצה

הוספת איש קשר חיצוני לקבוצת תפוצה (DG) היא תהליך בן שני שלבים:
  
1. צור איש קשר של דואר עבור המשתמש החיצוני:
    
    1. במרכז הניהול, עבור אל הדף **Users**'  >  [אנשי קשר](https://admin.microsoft.com/adminportal/home#/Contact) של משתמשים '. 
    
    2. בחר **הוסף איש קשר**.
    
    3. הקלד את המידע עבור איש הקשר שלך ובחר **הוסף**.
    
2. הוסף את איש הקשר לדואר ל-DG:
    
    1. במרכז הניהול, עבור אל הדף קבוצות **קבוצות**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. חפש את DG שאליה ברצונך להוסיף את המשתמש החיצוני ובחר אותו כדי לפתוח את תיבת הדו עריכה.
    
    3. בכרטיסיה **חברים** , בחר **הצג הכל ונהל את החברים**. 
    
    4. בחר **הוסף חברים**.
    
    5. בחר את איש הקשר לדואר שיצרת בשלב הקודם ולאחר מכן בחר **שמור**.
    
אם לאחר ביצוע שלבים אלה, משתמשים חיצוניים אינם יכולים לשלוח הודעות דואר אלקטרוני ל-DG או לא לקבל הודעות דואר אלקטרוני ממנו, ייתכן ש-DG מסומנת רק לאפשר הודעות דואר אלקטרוני ממשתמשים פנימיים. באפשרותך לבדוק תצורה זו ולפתור אותה בהתאם להוראות [כאן](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **הערה:** הוראות אלה אינן חלות אם הסוג של הקבוצה הוא "Microsoft 365 group" במקום "הקבוצה תפוצה". במקרה זה, באפשרותך להוסיף את המשתמש החיצוני ישירות לקבוצה מ-Outlook. מידע מפורט בנושא Microsoft 365 קבוצות האורחים וכן הוראות להוספת אורחים חיצוניים ניתן למצוא [במאמר זה](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  