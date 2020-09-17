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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806040"
---
# <a name="upgrade-azure-ad-connect"></a>התחברות לשדרוג תכלת לספירה

כברירת מחדל, שדרוג אוטומטי זמין עבור התחברות של תכלת לספירה, המסייעת לך להבטיח שאתה מפעיל את הגירסה העדכנית ביותר. כדי לאמת את הגדרות השדרוג האוטומטיות, השתמש ב **-Cmdlet Get-ADSyncAutoUpgrade** ב-תכלת AD PowerShell. ה-cmdlet יחזור לאחד מהערכים הבאים:

- **זמין**: שדרוג אוטומטי מופעל.

- לא **זמין**: שדרוג אוטומטי אינו זמין.

- **מושעה**: המערכת כבר אינה זכאית לקבל שדרוגים אוטומטיים. לא ניתן לקבוע את התצורה של ערך זה; היא מוגדרת על-ידי המערכת.

לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

כדי להוריד את הגירסה העדכנית ביותר של תכלת AD Connect, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
