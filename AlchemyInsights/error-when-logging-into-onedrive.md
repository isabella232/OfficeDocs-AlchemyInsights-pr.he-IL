---
title: 0x8004de40 בעת הפעלת OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946580"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 בעת הפעלת OneDrive

אם אתה מקבל הודעת **0x8004de40 בעת** כניסה ל- OneDrive, אתחל מחדש את המחשב בזמן שאתה מחובר לתחום שלך בעבודה או בבית הספר. אם אתה מקבל שגיאה זו לאחר אתחול מחדש, נסה זאת בזמן שאתה מחובר לתחום שלך בעבודה או בבית הספר:

1. לחץ על התחל והקלד **cmd** **או שורת פקודה**  בתיבת החיפוש, לחץ באמצעות לחצן העכבר הימני על אפליקציית שורת הפקודה ובחר  **הפעל כמנהל מערכת**. אם תתבקש לספק סיסמת מנהל מערכת או אישור, הקלד את הסיסמה או לחץ על **אפשר**.  

2. בחלון שורת הפקודה, הקלד **dsregcmd /leave**  ולהמתין להשלמת הפקודה. לאחר מכן **הקלד dsregcmd /join** ולהמתין להשלמת הפקודה.
3. אתחל מחדש את המחשב.
