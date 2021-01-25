---
title: מיפוי תכונות של הקצאת משתמשים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949763"
---
# <a name="user-provisioning-attribute-mapping"></a>מיפוי תכונות של הקצאת משתמשים

1. כדי לפתור בעיות ידועות במיפוי התכונות, ראה [מיפויי תכונות](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft תכלת Active Directory (AD) מספק תמיכה עבור הקצאת משתמשים ליישומי SaaS של ספקים חיצוניים כגון Salesforce, G Suite ואחרים. אם אתה מאפשר הקצאת משאבים עבור יישום של SaaS של ספק חיצוני, פורטל התכלת קובע את ערכי התכונות שלו באמצעות מיפויי תכונות. כדי ללמוד כיצד להתאים אישית את התכונה המוגדרת כברירת מחדל-מיפויים, ראה [התאמה אישית של תכונת הקצאת משתמשים-מיפויים עבור יישומי SaaS ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - לקבלת מידע נוסף אודות הקצאת משאבים של SaaS app, ראה [מהי הקצאת משתמשים אוטומטית של saas app בתכלת לספירה?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. בעת התאמה אישית של תכונה-מיפויים עבור הקצאת משאבים, ייתכן שתגלה שהתכונה שברצונך למפות אינה מופיעה ברשימה תכונת המקור. [סינכרון תכונה ממדריך הכתובות המקומי של Active Directory לכיוון תכלת ad לצורך הקצאת מאמר ליישום](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) מראה לך כיצד להוסיף את התכונה החסרה על-ידי סינכרון מהמודעה המקומית שלך ל-תכלת ad.
