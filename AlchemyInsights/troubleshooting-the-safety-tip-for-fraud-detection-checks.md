---
title: פתרון בעיות עצת בטיחות לאיתור הונאות
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955967"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>פתרון בעיות עצת בטיחות לאיתור הונאות

אם אתה מקבל הודעת עצת בטיחות "השולח נכשל בזיהוי ההונאה שלנו ו ייתכן שהוא אינו מי שהוא נראה", השולח לא הצליח להעביר בדיקת אימות DKIM או SPF. השיטה הטובה ביותר לפתור בעיה זו היא שהשולח יאשר את עצמו. אם השולח שולח בשמך, עליך לאשר אותו על-ידי הוספת כתובת ה- IP של השולח אל רשומת ה- SPF שלך.
  
ראה [פתרון בעיות באדום (חשוד) עצת בטיחות לאיתור הונאות לקבלת](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) מידע נוסף.
  
להלן כמה קישורים אחרים ה יכולים לעזור:
  
- [כיצד Microsoft משתמשת במסגרת מדיניות השולח (SPF) כדי למנוע תיפוף](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [הגדרת SPF כדי לסייע במניעת תיפוך](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
