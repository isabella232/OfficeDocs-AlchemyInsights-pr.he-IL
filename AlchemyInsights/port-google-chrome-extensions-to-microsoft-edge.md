---
title: הרחבות יציאה של Google Chrome ל-Microsoft Edge (כרומיום)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677880"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>הרחבות יציאה של Google Chrome ל-Microsoft Edge (כרומיום)

קל יותר להעביר את [הרחבות Google Chrome ל-Microsoft Edge (כרומיום)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). ברוב המקרים, דרושות רק שינויים מינימליים כדי לבצע הרחבות אלה ב-Microsoft Edge.

רכיבי ה-Api של ההרחבה ומפתחות המניפסט הנתמכים על-ידי Google Chrome תואמים לקוד עם Microsoft Edge. עם זאת, Microsoft Edge אינו תומך ברכיבי ה-Api של ההרחבה chrome. gcm, chrome. identity. getAccounts, chrome. identity. getAuthToken ו-chrome. instanceID.