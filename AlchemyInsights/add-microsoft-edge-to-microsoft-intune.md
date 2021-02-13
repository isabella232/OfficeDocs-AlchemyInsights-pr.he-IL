---
title: הוספת Microsoft Edge ל-Microsoft intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194509"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="625b5-102">הוספת Microsoft Edge ל-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="625b5-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="625b5-103">כדי שתוכל לפרוס, להגדיר, לנטר ולהגן על Microsoft Edge עבור Windows 10, תחילה עליך להוסיף אותו ל-Microsoft intune.</span><span class="sxs-lookup"><span data-stu-id="625b5-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="625b5-104">המנגינה תומכת ב-Microsoft Edge 77 ובגירסאות מתקדמות יותר.</span><span class="sxs-lookup"><span data-stu-id="625b5-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="625b5-105">התכונה ' כוונון ' תזהה את כל ההתקנות הקיימות מראש של Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="625b5-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="625b5-106">אם Microsoft Edge מותקן בהקשר של המשתמש, התקנת מערכת תחליף את ההתקנה בהקשר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="625b5-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="625b5-107">אם Microsoft Edge מותקן בהקשר מערכת, הצלחת ההתקנה תדווח.</span><span class="sxs-lookup"><span data-stu-id="625b5-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="625b5-108">מותקן מראש של Microsoft Edge 77 וגירסאות מתקדמות יותר, עבור כל הערוצים בהקשר המשתמש, יוחלפו ב-Microsoft Edge המותקנת בהקשר המערכת.</span><span class="sxs-lookup"><span data-stu-id="625b5-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="625b5-109">**תנאי**</span><span class="sxs-lookup"><span data-stu-id="625b5-109">**Prerequisite**</span></span>

<span data-ttu-id="625b5-110">Windows 10 גירסה 1709 ואילך</span><span class="sxs-lookup"><span data-stu-id="625b5-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="625b5-111">**השלבים להוספת קצה למנגינה**</span><span class="sxs-lookup"><span data-stu-id="625b5-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="625b5-112">[קבע את תצורת היישום בתוך המנגינה](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="625b5-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="625b5-113">[קביעת התצורה של פרטי האפליקציה](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="625b5-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="625b5-114">[קביעת התצורה של הגדרות האפליקציה](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="625b5-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="625b5-115">[בחר את תגי הטווח (אופציונלי)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="625b5-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="625b5-116">[הוסף את האפליקציה](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="625b5-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="625b5-117">לקבלת עזרה נוספת, ראה [פתרון בעיות](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="625b5-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




