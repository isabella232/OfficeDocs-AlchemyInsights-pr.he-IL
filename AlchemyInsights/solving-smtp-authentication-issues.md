---
title: פתרון בעיות אימות SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826416"
---
# <a name="solving-smtp-authentication-issues"></a>פתרון בעיות אימות SMTP

אם אתה מקבל שגיאות 5.7.57 או 5.7.3 בעת ניסיון לשלוח דואר אלקטרוני מסוג SMTP ולאמת עם לקוח או יישום, עליך לבדוק כמה דברים:

- ייתכן שהגשת SMTP מאומתת אינה זמינה דייר, או בתיבת הדואר שאתה מנסה להשתמש בה (בדוק את שתי ההגדרות). כדי לקרוא עוד, ראה [הפיכת הגשת SMTP של לקוח מאומת לזמינה או ללא זמינה.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- בדוק אם [ברירות המחדל של Azure Security](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) זמינות עבור הדייר שלך; אם אפשרות זו זמינה, אימות SMTP באמצעות אימות בסיסי (המכונה גם מדור קודם; פעולה זו תשתמש בשם משתמש וסיסמה) תיכשל.
