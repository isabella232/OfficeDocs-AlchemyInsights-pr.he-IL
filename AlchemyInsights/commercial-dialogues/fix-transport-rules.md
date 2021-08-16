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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034755"
---
# <a name="fix-transport-rules"></a>תיקון כללי תעבורה

כלל זרימת דואר מותאם אישית השפיע על הודעה זו. כדי לסקור את הכלל המדויק, ביצוע הפעולות הבאות:

1. בתוצאות ההגשה, תחת **מידע נוסף**, שים לב ל- **GUID** או **לשם המדיניות**.
2. הפעל Exchange ניהול מעטפת. לקבלת מידע נוסף, ראה [פתיחת Exchange ניהול.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. הפעל פקודה זו (באמצעות GUID מהשליחה שלך):  **Get-TransportRule -identity "GUID" | fl * Description***
4. סקור את התיאור כדי לראות את התנאים שהוגדרו שהשפיעו על ההודעה.

כדי ללמוד עוד, ראה [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
