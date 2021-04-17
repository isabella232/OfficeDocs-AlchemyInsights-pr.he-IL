---
title: פתרון בעיות של תיאור הבטיחות עבור בדיקת זיהוי הונאות
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834732"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>פתרון בעיות של תיאור הבטיחות עבור בדיקת זיהוי הונאות

אם אתה מקבל עצה בטיחותית שאומרת "השולח נכשל בזיהוי ההונאה שלנו ו ייתכן שהוא אינו מי שהוא נראה", השולח לא הצליח להעביר בדיקת אימות DKIM או SPF. השיטה הטובה ביותר לפתור בעיה זו היא שהשולח יאשר את עצמו. אם השולח שולח בשמך, עליך לאשר אותו על-ידי הוספת כתובת ה- IP של השולח אל רשומת ה- SPF שלך.
  
לקבלת [מידע נוסף, ראה פתרון בעיות של עצה הבטיחות האדומה (החשודה)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) לאיתור הונאות.
  
להלן כמה קישורים אחרים ה יכולים לעזור:
  
- [כיצד Microsoft משתמשת במסגרת מדיניות השולח (SPF) כדי למנוע תיפוף](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [הגדרת SPF כדי לסייע במניעת תיפוך](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
