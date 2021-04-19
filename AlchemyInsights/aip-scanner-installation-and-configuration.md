---
title: 'סורק AIP: התקנה וקביעת תצורה'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821664"
---
# <a name="aip-scanner-installation-and-configuration"></a>סורק AIP: התקנה וקביעת תצורה

**כדי להתקין את סורק AIP, בצע את ההנחיות המומלצות**:

1. אם אתה משדרג ולא מבצע התקנה נקייה, ודא שעקבת אחר הקווים המנחים לשדרוג סורק [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) וללקוח תיוג מאוחד, ראה שדרוג [הסורק Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. ודא שאתה מציית לכל דרישות [הגדרות חומת האש ותשתית הרשת.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. ודא שמדיניות [זו מוגדרת לתיוג](https://docs.microsoft.com/azure/information-protection/configure-policy) אוטומטי או שיש לה תווית ברירת מחדל במדיניות.
4. ודא שסוג הקובץ הרלוונטי מוגדר עבור תווית/הגנה כמתואר בסוגי קבצים הנתמכים [על-ידי לקוח Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). בנוסף, אם ברצונך לשנות את אופן הפעולה המוגדר כברירת מחדל, בצע את ההנחיות הבאות: [שינוי רמת ההגנה המוגדרת כברירת מחדל של קבצים](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. ודא שחשבון המשתמש שהוגדר להפעיל את שירות הסורק כולל הרשאות לגשת לכל מאגרי מאגרים שהוגדרו.
6. אם אתה עדיין נתקל בבעיות, ייצא את יומני הסורק והוסף אותם לכרטיס התמיכה שלך.

**ייצוא יומנים של סורק הגנה על מידע של Azure**

1. נווט אל %localappdata%\Microsoft\MSIP תחת הקשר המשתמש שבו פועל שירות הסורק.
2. דחוס את כל התוכן תחת התיקיה MSIP.
3. שמור את יומני הרישום במיקום שלך וצרף אותם לבקשת השירות שלך.
4. באפשרותך גם להשתמש [בייצוא-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**לקבלת מידע נוסף, ראה**:
- [פריסת סורק Azure Information Protection כדי לסווג ולהגן באופן אוטומטי על קבצים](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [ציין את הפרמטר Token והשתמש בו עבור Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [הפעלת מחזור גילוי ו הצגת דוחות עבור הסורק](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [סקירת התיעוד של Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [דרישות עבור Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [הורד את לקוח Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
