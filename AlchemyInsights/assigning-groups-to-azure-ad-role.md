---
title: הקצאת קבוצות לתפקיד Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036241"
---
# <a name="assigning-groups-to-azure-ad-role"></a>הקצאת קבוצות לתפקיד Azure AD

כדי להקצות קבוצה של Azure AD עם מקור סמכות ב- Azure AD לתפקיד Azure AD, בצע את השלבים הבאים:

1. צור קבוצה חדשה - כדי ליצור קבוצה חדשה:

    a. היכנס למרכז הניהול של Azure AD עם הרשאות **מנהל תפקידים או** הרשאות **מנהל מערכת** כלליות.
    b. בחר **Azure Active Directory > קבוצות > כל הקבוצות > קבוצה חדשה**.
    c. צור את הקבוצה.

2. הקצה את התפקיד לקבוצה במהלך יצירת קבוצה או לאחר יצירת הקבוצה.

    a. כדי להקצות תפקיד לקבוצה בעת יצירת הקבוצה, ניתן להקצות לקבוצה את תפקידי **Azure AD** הדו-מצביים וליצור את הקבוצה.
    b. כדי להקצות תפקיד לקבוצה לאחר יצירתה, נווט אל הכרטיסיה תפקידים שהוקצו עבור הקבוצה החדשה שנוצרה והקצה את התפקיד לקבוצה.   

**ניהול חברות בקבוצה שהוקצתה לתפקיד Azure AD**

כדי למנוע העלאת הרשאות, כברירת מחדל, רק מנהלי תפקידים מיוחסים ומנהלי מערכת כלליים יכולים לשנות את החברות בקבוצה שהוקצתה לתפקיד. עם זאת, הם יכולים לבחור להקצות בעלים עבור קבוצה כזו ולהקצות משימה זו.

לקבלת פרטים נוספים על הקצאת קבוצות ענן לתפקידי Azure AD, ראה [הקצאת תפקידי AD לקבוצת ענן](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). לקבלת פרטים נוספים על פתרון בעיות בתפקידים שהוקצו לקבוצות ענן, ראה [פתרון בעיות בתפקידים שהוקצו לקבוצות ענן](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





