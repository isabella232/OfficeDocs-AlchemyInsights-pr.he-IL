---
title: שנה את Microsoft Edge באמצעות משתני מדריך הנתונים במקום נתיבים בקידוד קשיח
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035818"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>שנה את Microsoft Edge באמצעות משתני מדריך הנתונים במקום נתיבים בקידוד קשיח

לדוגמה, ב-Windows, כדי לאחסן את נתוני הפרופיל תחת נתוני היישום המקומי של המשתמש, במקום במיקום ברירת המחדל, הגדר את מדיניות *UserDataDir* ל- **$ {local_app_data} \Edge\Profile**.

לקבלת מידע נוסף, ראה [יצירת משתני מדריך נתונים של משתמשים ב-Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).