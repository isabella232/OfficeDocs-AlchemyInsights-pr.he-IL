---
title: הסרת שירות הרקע עבור Microsoft Search ב-Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816200"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>הסרת שירות הרקע עבור Microsoft Search ב-Bing

כדי להסיר את שירות הרקע עבור Microsoft Search ב-Bing, באפשרותך לנסות את התרופות הבאות:

1. כדי לחזור להגדרות מנוע החיפוש המקוריות, בצע את הפעולות הבאות:

    מ. החלף **[את](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) השימוש Bing כמנוע החיפוש המוגדר כברירת מחדל**.

    b. [עבור אל מרכז הניהול של Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ונקה את ההגדרה המשפיעה על כל המשתמשים בארגון שלך.

2. כדי להסיר את שירות הרקע ממכשיר בודד, בצע את המשימות הבאות:

    מ. בחר **לוח הבקרה > תוכניות > תוכניות ותכונות**.

    b. לחץ **באמצעות לחצן** העכבר הימני על Microsoft Search ב-Bing תחת רשימת התוכניות המותקנות ולאחר מכן לחץ על **הסר התקנה**.

3. כדי להסיר את שירות הרקע ממכשירים מרובים בארגון שלך, היכנס כמנהל מערכת והפעיל את הפקודה הבאה בקובץ script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
