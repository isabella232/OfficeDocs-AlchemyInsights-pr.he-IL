---
title: פתרון בעיות בבדיקת זיהוי הונאה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658411"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>פתרון בעיות בבדיקת זיהוי הונאה

אם אתה מקבל עצת בטיחות המציינת ש-"השולח נכשל בבדיקות זיהוי ההונאה שלנו וייתכן שהוא לא מי שהם נראים", השולח לא הצליח להעביר בדיקות אימות של DKIM או SPF. השיטה הטובה ביותר לפתרון זו היא שהשולח יאשר את עצמו. אם השולח שולח בשמך, עליך לאשר אותם על-ידי הוספת כתובת ה-IP של השולח לרשומת SPF.
  
לקבלת מידע נוסף, ראה [פתרון בעיות בעצת הבטיחות האדומה (חשודה) לאיתור הונאה](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
להלן כמה קישורים אחרים שיכולים לעזור:
  
- [כיצד Microsoft משתמשת במסגרת מדיניות השולח (SPF) כדי למנוע זיופים](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [הגדרת SPF כדי לסייע במניעת זיופים](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
