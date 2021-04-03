---
title: הרחבות Google Chrome של Port ל- Microsoft Edge (כרום)
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
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505285"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>הרחבות Google Chrome של Port ל- Microsoft Edge (כרום)

קל לתפור [הרחבות Google Chrome ל- Microsoft Edge (כרום)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). ברוב המקרים, נדרשים רק שינויים מינימליים כדי להפעיל הרחבות אלה ב- Microsoft Edge.

ממשקי ה- API של ההרחבה ומפתחות מניפסט הנתמכים על-ידי Google Chrome תואמים לקוד עם Microsoft Edge. עם זאת, Microsoft Edge אינו תומך ב- API של ההרחבה chrome.gcm , chrome.identity.getAccounts , chrome.identity.getAuthToken ו- chrome.instanceID.