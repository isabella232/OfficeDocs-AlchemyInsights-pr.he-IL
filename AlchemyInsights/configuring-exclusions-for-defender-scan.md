---
title: קביעת התצורה של אי-הכללות עבור סריקת ATP של Microsoft Defender
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
ms.openlocfilehash: 0b64217062aadea22afe1aa17748a5f38b9f1cd6c59adc54345afe3c6f12bdc2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900333"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>קביעת התצורה של אי-הכללות עבור סריקת ATP של Microsoft Defender

באופן כללי, באפשרותך לא לכלול סיומות קבצים מסוימות ומיקום תיקיה מסריקות ATP של Microsoft Defender. באפשרותך גם לקבוע תצורה של אי-הכללות עבור קבצים שנפתחו על-ידי תהליכים מסוימים. לקבלת מידע נוסף, ראה קביעת תצורה [ואמת של אי-הכללות בהתבסס](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) על סיומת קובץ ומיקום תיקיה והגדרה [של אי-הכללות עבור קבצים שנפתחו על-ידי תהליכים](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

כדי לקבוע תצורה של **אי-הכללות עבור Windows Server 2016 ו- 2019,** [ראה קביעת תצורה של אנטי-וירוס של Microsoft Defender אי-הכללות ב- Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).

**Mac**

לקבלת פרטים על סוגי אי-הכללה נתמכים וקביעת תצורה של רשימה של אי-הכללות עבור Mac, ראה סוגי [אי-הכללה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) נתמכים ואופן קביעת התצורה [של רשימת אי-הכללות.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)

**הערה** באפשרותך גם לאמת רשימות אי-הכללה באמצעות קובץ מחשב ה- EICAR. לקבלת מידע נוסף, [ראה אימות רשימות אי-הכללה עם קובץ מחשב של EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

לקבלת פרטים על סוגי אי-הכללה נתמכים וקביעת התצורה של רשימה של אי-הכללות עבור Linux, ראה סוגי [אי-הכללה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) נתמכים והגדרה של אי-הכללות עבור [Microsoft Defender ATP עבור Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)

**הערה** באפשרותך גם לאמת רשימות אי-הכללה באמצעות קובץ מחשב ה- EICAR. לקבלת מידע נוסף, [ראה אימות רשימות אי-הכללה עם קובץ מחשב של EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 