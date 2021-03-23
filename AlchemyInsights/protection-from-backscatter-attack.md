---
title: הגנה מפני התקפה של Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036072"
---
# <a name="protection-from-backscatter-attack"></a>הגנה מפני התקפה של Backscatter

Backscatter הוא דוחות אי-מסירה (המכונים גם ' הודעות ' Ndr ' או ' הקפץ ') שאתה מקבל עבור הודעות שלא שלחת. שולחי הודעות זבל מזייפים (מזייפים) את הכתובת **מאת:** ההודעות שלהם, ולעתים קרובות הם משתמשים בכתובות דואר אלקטרוני אמיתיות כדי להעניק אמינות להודעות שלהם. כך, כאשר שולחי הודעות זבל שולחים הודעות לנמענים שאינם קיימים, שרת הדואר האלקטרוני של היעד מרומה למעשה להחזרת ההודעה שאינה ניתנת למסירה בהודעת NDR לשולח המזייף בכתובת **From:** .

מידע נוסף ניתן למצוא ב- [Backscatter ב-EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**הפעלת הגנה מפני Backscatter**

כדי להפוך הגנה של Backscatter לזמינה, בצע את הנתיב שלהלן.

**protection.office.com > מדיניות ניהול האיום > > ספאם > בחירת מדיניות מסנן דואר הזבל ועריכת מדיניות > מאפייני דואר זבל > סימון כהודעת זבל > NDR backscatter > הגדר אותה "On"**

אם אתה סבור שהחשבון נחשף, עיין בפרטים הבאים:

- [תגובה לחשבון דואר אלקטרוני שנחשף](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [הסרת משתמשים חסומים מפורטל המשתמשים המוגבלים ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



