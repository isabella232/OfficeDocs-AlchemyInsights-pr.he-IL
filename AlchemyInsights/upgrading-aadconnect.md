---
title: 932 שדרוג AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104813"
---
# <a name="upgrade-azure-ad-connect"></a>שדרוג Azure AD התחברות

כברירת מחדל, שדרוג אוטומטי זמין עבור Azure AD התחברות, מה שמסייע להבטיח שאתה משתמש בגירסה העדכנית ביותר. כדי לאמת את הגדרות השדרוג האוטומטי, השתמש **ב- cmdlet Get-ADSyncAutoUpgrade** ב- Azure AD PowerShell. ה- cmdlet יחזיר אחד מהערכים הבאים:

- **זמין**: שדרוג אוטומטי זמין.

- **לא** זמין : שדרוג אוטומטי אינו זמין.

- **מושעה**: המערכת אינה זכאית עוד לקבל שדרוגים אוטומטיים. לא ניתן לקבוע את התצורה של ערך זה; הוא מוגדר על-ידי המערכת.

לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

כדי להוריד את הגירסה העדכנית ביותר של Azure AD התחברות, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
