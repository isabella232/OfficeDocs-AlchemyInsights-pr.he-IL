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
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="ed0c9-102">הרחבות יציאה של Google Chrome ל-Microsoft Edge (כרומיום)</span><span class="sxs-lookup"><span data-stu-id="ed0c9-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="ed0c9-103">קל יותר להעביר את [הרחבות Google Chrome ל-Microsoft Edge (כרומיום)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="ed0c9-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="ed0c9-104">ברוב המקרים, דרושות רק שינויים מינימליים כדי לבצע הרחבות אלה ב-Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="ed0c9-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="ed0c9-105">רכיבי ה-Api של ההרחבה ומפתחות המניפסט הנתמכים על-ידי Google Chrome תואמים לקוד עם Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="ed0c9-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="ed0c9-106">עם זאת, Microsoft Edge אינו תומך ברכיבי ה-Api של ההרחבה chrome. gcm, chrome. identity. getAccounts, chrome. identity. getAuthToken ו-chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="ed0c9-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>