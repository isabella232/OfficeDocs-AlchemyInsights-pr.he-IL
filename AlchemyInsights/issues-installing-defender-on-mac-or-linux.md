---
title: בעיות בהתקנת Microsoft Defender ב- Mac או ב- Linux
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
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013245"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>בעיות בהתקנת Microsoft Defender ב- Mac או ב- Linux

**Mac**

- ודא שדרישות המערכת יתקינו לפני התקנת Microsoft Defender ATP עבור Mac. לקבלת מידע נוסף, ראה [כיצד להתקין את Microsoft Defender ATP עבור Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- סקור את המידע בקובץ: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- ודא שדרישות המערכת יתקינו לפני התקנת Microsoft Defender ATP עבור Linux. לקבלת מידע נוסף, [ראה כיצד להתקין את MDATP עבור Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- כדי לוודא ששירות MDATP פועל, ראה [ההתקנה נכשלה.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    כדי לפתור בעיות ולפתור בעיות אם השירות אינו פועל, ראה [שלבים לפתרון בעיות אם שירות mdatp אינו פועל.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- לקבלת שלבים כדי לבדוק את תצורת הלקוח, אשר מאמתת את תקינות המוצר, ולהפעיל זיהוי מחשב בקובץ הטקסט של EICAR, ראה [תצורת לקוח](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **הערה** לקבלת רשימה של מערכות קבצים נתמכות עבור פעילות בגישה, ראה [Microsoft Defender ATP עבור Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).