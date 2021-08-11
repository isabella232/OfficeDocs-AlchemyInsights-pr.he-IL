---
title: בדיקת תצורת IRM עבור יכולות OME חדשות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812436"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>בדיקת תצורת IRM עבור יכולות OME חדשות

כדי לוודא שהדייר Microsoft 365 שלך מוגדר לשימוש ביכולות OME חדשות, הפעל את כלי ה- cmdlet הבאים [בזמן שאתה מחובר ל- Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell):


1. בדוק את תצורת IRM של הדייר שלך על-ידי הפעלת `Get-IRMConfiguration` . ודא שערכים אלה מוגדרים ל- **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. באמצעות התחום, כתובת השולח ונמען, הפעל `Test-IRMConfiguration` . אם מחשב אינה תחלוף, בדוק את תצורת IRM שלך.

לקבלת מידע נוסף אודות אימות תצורת IRM, ראה אימות תצורה [חדשה של OME ב- Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).