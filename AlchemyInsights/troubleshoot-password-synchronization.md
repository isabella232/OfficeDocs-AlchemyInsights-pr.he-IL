---
title: פתרון בעיות בסינכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664927"
---
# <a name="troubleshoot-password-synchronization"></a>פתרון בעיות בסינכרון סיסמאות

כדי לפתור בעיות בסינכרון סיסמאות, התחל באמצעות משימת התחברות זו לפתרון בעיות כדי לקבוע מדוע סיסמאות אינן מסונכרנות. כדי להתחיל, עבור אל [ניהול סינכרון ישיר](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. פתח הפעלה חדשה של Windows PowerShell בשרת החיבור של תכלת לספירה ובחר באפשרות **הפעל כמנהל** .

2. הפעיל את Set-ExecutionPolicy RemoteSigned או Set-ExecutionPolicy בלתי מוגבל.

3. הפעל את אשף ההתחברות של תכלת לספירה.

4. עבור אל דף המשימות הנוספות > **פתור את הבעיות**  >  **הבאות**.

5. בחר **הפעל** כדי לפתוח את תפריט פתרון בעיות של PowerShell.

6. בחר באפשרות **פתרון בעיות בסינכרון סיסמאות**.

    הבעיה היא בדרך כלל שסיסמה אינה מסונכרנת עבור חשבון משתמש ספציפי.

    **הערות** סינכרון סיסמאות נכשל אם סינכרון הסיסמאות האחרון שהצליח היה לפני זמן מה.

לקבלת עזרה נוספת בפתרון בעיות בסינכרון סיסמאות, ראה [פתרון בעיות בסינכרון hash של סיסמאות באמצעות הסינכרון של תכלת AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).