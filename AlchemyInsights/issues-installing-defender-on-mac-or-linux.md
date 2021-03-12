---
title: בעיות בהתקנת Microsoft Defender ב-Mac או ב-Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713544"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>בעיות בהתקנת Microsoft Defender ב-Mac או ב-Linux

**Mac**

- ודא שדרישות המערכת נפגשות לפני התקנת Microsoft Defender ATP עבור Mac. לקבלת מידע נוסף, ראה [כיצד להתקין את Microsoft DEFENDER ATP עבור Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- סקור את המידע בקובץ: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- ודא שדרישות המערכת נפגשות לפני התקנת Microsoft Defender ATP עבור Linux. לקבלת מידע נוסף, ראה [כיצד להתקין את Microsoft DEFENDER ATP עבור Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- כדי לוודא ששירות MDATP פועל, ראה [ההתקנה נכשלה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    כדי לפתור בעיות ולפתור בעיות אם השירות אינו פועל, ראה [שלבים לפתרון בעיות אם השירות של mdatp אינו פועל](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- לקבלת שלבים לבדיקת תצורת הלקוח, המאמתת את תקינות המוצר ולהפעלת בדיקת זיהוי בקובץ הטקסט של EICAR, ראה [תצורת לקוח](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **הערה** לקבלת רשימה של מערכות קבצים נתמכות עבור פעילות בגישה, ראה [Microsoft DEFENDER ATP עבור Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).