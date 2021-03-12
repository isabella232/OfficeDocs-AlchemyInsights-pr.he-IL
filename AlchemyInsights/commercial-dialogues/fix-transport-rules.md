---
title: תיקון כללי תעבורה
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746737"
---
# <a name="fix-transport-rules"></a>תיקון כללי תעבורה

כלל זרימת דואר מותאם אישית השפיע על הודעה זו. כדי לסקור את הכלל המדויק, בצע את הפעולות הבאות:

1. בתוצאות המסירה, תחת **מידע נוסף**, רשום את ה- **GUID** או את **שם המדיניות**.
2. הפעל את מעטפת ניהול Exchange. לקבלת מידע נוסף, ראה [פתיחת מעטפת ניהול Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
3. הפעיל פקודה זו (באמצעות ה-GUID מתוך השליחה שלך):  **Get-TransportRule-identity "GUID" | fl * Description***
4. סקור את התיאור כדי לראות את התנאים שתצורתם נקבעה והשפיעו על ההודעה.

לקבלת מידע נוסף, ראה [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
