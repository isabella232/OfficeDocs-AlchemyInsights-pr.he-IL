---
title: שגיאת 0x8004de40 בעת הפעלת OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823049"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>שגיאת 0x8004de40 בעת הפעלת OneDrive

אם אתה מקבל הודעת שגיאה **0x8004de40** בעת כניסה ל-OneDrive, אתחל מחדש את המחשב בזמן שאתה מחובר לתחום בעבודה או בבית הספר. אם אתה מקבל שגיאה זו לאחר אתחול מחדש, נסה זאת בזמן שאתה מחובר לתחום בעבודה או בבית הספר:

1. לחץ על התחל והקלד **cmd** או **שורת פקודה**  בתיבת החיפוש, לחץ באמצעות לחצן העכבר הימני על יישום שורת הפקודה ובחר  **הפעל כמנהל** . אם אתה מתבקש להזין סיסמת מנהל מערכת או אישור, הקלד את הסיסמה או לחץ על **אפשר** .  

2. בחלון שורת הפקודה, הקלד **dsregcmd/leave**  והמתן להשלמת הפקודה. לאחר מכן הקלד **dsregcmd/join** והמתן להשלמת הפקודה.
3. הפעל מחדש את המחשב.
