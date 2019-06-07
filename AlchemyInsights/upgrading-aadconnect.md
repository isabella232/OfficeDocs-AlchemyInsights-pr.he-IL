---
title: AADConnect שדרוג 932
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757292"
---
# <a name="upgrade-azure-ad-connect"></a>שדרוג AD תכלת הרקיע להתחבר

כברירת מחדל, שדרוג אוטומטי זמין עבור התחברות AD תכלת הרקיע, המסייעת להבטיח לך אתה מפעיל את הגירסה העדכנית ביותר. כדי לוודא את הגדרות השדרוג האוטומטי, השתמש cmdlet **Get-ADSyncAutoUpgrade** ב- AD PowerShell תכלת הרקיע. ה-cmdlet תחזיר את אחד הערכים הבאים: 

- **זמין**: שדרוג אוטומטי מופעלת.

- **זמין**: שדרוג אוטומטי אינו זמין.

- **מושעה**: המערכת כבר לא זכאי לקבל שדרוגים אוטומטיים. אין באפשרותך להגדיר ערך זה; הוא מוגדר על-ידי המערכת. 

לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

כדי להוריד את הגירסה העדכנית ביותר של חיבור AD תכלת הרקיע, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
