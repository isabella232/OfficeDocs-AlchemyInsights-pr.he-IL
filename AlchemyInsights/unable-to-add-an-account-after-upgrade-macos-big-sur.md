---
title: לא ניתן להוסיף חשבון לאחר השדרוג ל- macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506478"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>לא ניתן להוסיף חשבון לאחר השדרוג ל- macOS 11.6 Big Sur

לאחר השדרוג ל- macOS 11.6, ייתכן שהחשבון OneDrive שלך לעבודה או לבית הספר או לחשבון OneDrive האישי שלך לא יופיע ברשימת החשבונות שלך, וייתכן שלא תוכל להיכנס לחשבון שני מתוך היישום.

פותח תיקון עבור בעיה זו. תחילה, קבע אם אתה משתמש בגירסה עצמאית או ב- App Store של OneDrive:

- בחר את OneDrive הענן בתיבת התפריטים > **עזרה & הגדרות**  >    >  **העדפות אודות**. אם מספר הגירסה אינו כולל **(עצמאי)**, יש לך את גירסת App Store של המוצר.

אם אתה משתמש בגירסה עצמאית של OneDrive, הפעל מחדש את המחשב ועדכן OneDrive אוטומטי לגירסת Build שבה נפתרה בעיה זו. אם ברצונך להתקין את ה- Build באופן ידני, [הורד קובץ.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)זה , בטל את ההעתקה של הקובץ והעתק את יישום OneDrive לתיקיה Applications (על-ידי החלפת יישום OneDrive הקיים).

אם אתה משתמש בגירסה של App Store, שקול להתקין את הגירסה הבודדת של OneDrive. גירסה זו פועלת באופן זהה לגירסת App Store, אך מאפשרת ל- Microsoft להציע עדכונים במהירות רבה יותר למשתמשים ומחברת אותם לגירסה הכוללת את התיקון לבעיה זו.

1. הורד את הגירסה הבודדת של [OneDrive הכוללת את התיקון](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. בטל את ההעתקה של הקובץ והעתק את OneDrive לתיקיה Applications (על-ידי החלפת יישום OneDrive הקיים).

אם עליך להשתמש בגירסה של App Store, המתן עד ש- App Store ישחרר גירסה של היישום הכוללת את התיקון. למרבה הצער, ל- Microsoft אין אפשרות לקיים תאריך משוער להפצה של גירסה קבועה מ- App Store.


