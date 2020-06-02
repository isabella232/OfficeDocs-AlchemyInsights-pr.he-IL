---
title: פתרון בעיות בעצת הבטיחות עבור בדיקות זיהוי הונאות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504984"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>פתרון בעיות בעצת הבטיחות עבור בדיקות זיהוי הונאות

אם אתה מקבל עצה בטיחות שאומרת "השולח נכשל בבדיקות ההונאה שלנו וייתכן שהוא אינו מי שהם נראים", אזי השולח לא הצליח לעבור בדיקות אימות DKIM או SPF. השיטה הטובה ביותר לפתרון זה היא שהשולח יאשר את עצמו. אם השולח שולח בשמך, עליך לאשר אותם על-ידי הוספת כתובת ה-IP של השולח לרשומת SPF.
  
ראה [פתרון בעיות בעצת הבטיחות האדומה (החשודה) לקבלת מידע נוסף על בדיקות זיהוי הונאות](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
להלן כמה קישורים אחרים שיכולים לעזור:
  
- [כיצד משתמש Microsoft במסגרת מדיניות השולח (SPF) כדי למנוע זיופים](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [הגדר SPF כדי לסייע במניעת זיופים](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
