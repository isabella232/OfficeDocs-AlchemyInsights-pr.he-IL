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
# <a name="fix-transport-rules"></a><span data-ttu-id="37f9e-102">תיקון כללי תעבורה</span><span class="sxs-lookup"><span data-stu-id="37f9e-102">Fix transport rules</span></span>

<span data-ttu-id="37f9e-103">כלל זרימת דואר מותאם אישית השפיע על הודעה זו.</span><span class="sxs-lookup"><span data-stu-id="37f9e-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="37f9e-104">כדי לסקור את הכלל המדויק, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="37f9e-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="37f9e-105">בתוצאות המסירה, תחת **מידע נוסף**, רשום את ה- **GUID** או את **שם המדיניות**.</span><span class="sxs-lookup"><span data-stu-id="37f9e-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="37f9e-106">הפעל את מעטפת ניהול Exchange.</span><span class="sxs-lookup"><span data-stu-id="37f9e-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="37f9e-107">לקבלת מידע נוסף, ראה [פתיחת מעטפת ניהול Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="37f9e-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="37f9e-108">הפעיל פקודה זו (באמצעות ה-GUID מתוך השליחה שלך):  **Get-TransportRule-identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="37f9e-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="37f9e-109">סקור את התיאור כדי לראות את התנאים שתצורתם נקבעה והשפיעו על ההודעה.</span><span class="sxs-lookup"><span data-stu-id="37f9e-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="37f9e-110">לקבלת מידע נוסף, ראה [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="37f9e-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
