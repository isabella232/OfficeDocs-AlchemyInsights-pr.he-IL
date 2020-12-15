---
title: שנה את Microsoft Edge באמצעות משתני מדריך הנתונים במקום נתיבים של קשיח
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677991"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>שנה את Microsoft Edge באמצעות משתני מדריך הנתונים במקום נתיבים של קשיח

לדוגמה, ב-Windows, כדי לאחסן את נתוני הפרופיל תחת נתוני היישום המקומי של המשתמש, במקום במיקום ברירת המחדל, הגדר את מדיניות **UserDataDir** ל- **$ {local_app_data} \Edge\Profile**. 

לקבלת מידע נוסף, ראה [יצירת משתני מדריך נתונים של משתמשים ב-Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).