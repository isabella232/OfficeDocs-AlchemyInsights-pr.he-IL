---
title: 'סורק AIP: התקנה וקביעת תצורה'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358097"
---
# <a name="aip-scanner-installation-and-configuration"></a>סורק AIP: התקנה וקביעת תצורה

**כדי להתקין את סורק AIP, בצע את ההנחיות המומלצות**:

1. אם אתה משדרג ולא מבצע התקנה נקייה, אנא ודא שעקבת אחר ההנחיות [לשדרוג הסורק הגנה מפני מידע תכלת](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ועבור לקוח מאוחד לתיוג, ראה [שדרוג סורק הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. ודא שאתה מציית לכל [הדרישות של חומות האש והגדרות התשתית הרשת](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. ודא [שפריטי המדיניות מוגדרים](https://docs.microsoft.com/azure/information-protection/configure-policy) לתיוג אוטומטי או שתווית ברירת מחדל מוגדרת במדיניות.
4. ודא שסוג הקובץ הרלוונטי מוגדר עבור תווית/הגנה כמתואר [בסוגי קבצים הנתמכים על-ידי לקוח ' הגנת מידע תכלת '](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). בנוסף, אם ברצונך לשנות את אופן הפעולה המוגדר כברירת מחדל, פעל לפי ההנחיות הבאות: [שינוי רמת ההגנה המהווה ברירת מחדל של קבצים](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. ודא שלחשבון המשתמש המוגדר להפעלת שירות הסורק יש הרשאות גישה לכל המאגרים שתצורתם נקבעה.
6. אם אתה עדיין נתקל בבעיות, אנא יצא את יומני הרישום של הסורק והוסף אותם לכרטיס התמיכה.

**ייצוא הגנה מידע תכלת הסורק יומנים**

1. נווט ל-%Localappנתונים\mvsip בהקשר המשתמש המפעיל את שירות הסורק.
2. לסגור את כל התוכן תחת התיקיה MSIP.
3. שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת השירות שלך.
4. אתה יכול גם להשתמש [ייצוא-AIPLogs-Onbeחצאי של](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**לקבלת מידע נוסף, ראה**:
- [פריסת הסורק הגנת מידע תכלת כדי לסווג ולהגן באופן אוטומטי על קבצים](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [ציון ושימוש בפרמטר Token עבור הגדרת אימות](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [הפעלת מחזור גילוי והצגת דוחות עבור הסורק](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [סקירת התיעוד של הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [דרישות להגנה מפני מידע תכלת](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [הורד את לקוח הגנת מידע תכלת](https://www.microsoft.com/download/details.aspx?id=53018)
