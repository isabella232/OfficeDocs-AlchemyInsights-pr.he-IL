---
title: קביעת התצורה של אי-הכללות עבור Microsoft Defender ATP סריקה
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543686"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>קביעת התצורה של אי-הכללות עבור Microsoft Defender ATP סריקה

באופן כללי, באפשרותך לא לכלול סיומות קבצים ומיקום תיקיה מסוימים Microsoft Defender ATP סריקות. באפשרותך גם לקבוע תצורה של אי-הכללות עבור קבצים שנפתחו על-ידי תהליכים מסוימים. לקבלת מידע נוסף, ראה קביעת תצורה [ואמת של אי-הכללות בהתבסס](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) על סיומת קובץ ומיקום תיקיה והגדרה [של אי-הכללות עבור קבצים שנפתחו על-ידי תהליכים](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

כדי לקבוע תצורה של **אי-הכללות עבור Windows Server 2016 ו- 2019,** [ראה קביעת תצורה של אנטי-וירוס של Microsoft Defender אי-הכללות ב- Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).

**Mac**

לקבלת פרטים על סוגי אי-הכללה נתמכים וקביעת תצורה של רשימה של אי-הכללות עבור Mac, ראה סוגי [אי-הכללה](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) נתמכים ואופן קביעת התצורה [של רשימת אי-הכללות.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)

**הערה** באפשרותך גם לאמת רשימות אי-הכללה באמצעות קובץ מחשב EICAR. לקבלת מידע נוסף, ראה [אימות רשימות אי-הכללות עם קובץ מחשב של EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

לקבלת פרטים על סוגי אי-הכללה נתמכים וקביעת התצורה של רשימה של אי-הכללות עבור Linux, ראה סוגי [אי-הכללה](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) נתמכים והגדרה של אי-הכללות [עבור Microsoft Defender ATP עבור Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)

**הערה** באפשרותך גם לאמת רשימות אי-הכללה באמצעות קובץ מחשב EICAR. לקבלת מידע נוסף, ראה [אימות רשימות אי-הכללות עם קובץ מחשב של EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 