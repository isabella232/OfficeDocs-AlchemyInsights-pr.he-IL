---
title: קביעת התצורה של פריטים שאינם מוכללים עבור סריקת Microsoft Defender ATP
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
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713574"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>קביעת התצורה של פריטים שאינם מוכללים עבור סריקת Microsoft Defender ATP

באופן כללי, באפשרותך לכלול הרחבות קבצים ומיקומי תיקיות מסוימים מסריקות Microsoft Defender ATP. באפשרותך גם להגדיר פריטים שאינם מוכללים עבור קבצים שנפתחו על-ידי תהליכים מסוימים. לקבלת מידע נוסף, ראה [קביעת תצורה ואימות של פריטים מוכללים בהתבסס על סיומת הקובץ ומיקום התיקיה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) [וקביעת תצורה של פריטים שאינם מוכללים עבור קבצים שנפתחו על-ידי תהליכים](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

כדי לקבוע תצורה של פריטים שאינם מוכללים עבור  **Windows server 2016 ו-2019**, ראה קביעת תצורה של הוראות הוראות הפעלה [של Microsoft Defender ב-windows server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).

**Mac**

לקבלת פרטים אודות סוגי אי-הכללה נתמכים וקביעת התצורה של רשימה של פריטים מובילים עבור Mac, ראה [סוגי](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) אי-הכללה נתמכים [וכיצד לקבוע את התצורה של רשימת הפריטים המפורטים](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).

**הערה** באפשרותך גם לאמת רשימות שאינן מוכללות באמצעות קובץ הבדיקה של EICAR. לקבלת מידע נוסף, ראה [אימות רשימות אי-הכללה באמצעות קובץ הבדיקה של EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

לקבלת פרטים אודות סוגי אי-הכללה נתמכים וקביעת התצורה של רשימה של פריטים מובילים עבור Linux, ראה סוגי אי- [הכללה נתמכים](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) [וקביעת תצורה ואימות של פריטים מוכללים עבור Microsoft Defender ATP עבור Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).

**הערה** באפשרותך גם לאמת רשימות שאינן מוכללות באמצעות קובץ הבדיקה של EICAR. לקבלת מידע נוסף, ראה [אימות רשימות אי-הכללה באמצעות קובץ הבדיקה של EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 