---
title: הפעלת פריסת האפליקציה של Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461869"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="5f6e2-102">הפעלת פריסת האפליקציה של Win32</span><span class="sxs-lookup"><span data-stu-id="5f6e2-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="5f6e2-103">Microsoft intune מאפשרת ליישומי Win32, כולל אך לא מוגבל ל-MSI ו-. EXE שיש לפרוס במכשירי Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="5f6e2-104">מנגנון הפריסה שנעשה בו שימוש דורש את הרחבת הניהול של ' שימוש ' (IME) להיות נוכח בהתקן היעד.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="5f6e2-105">ה-IME יותקן באופן אוטומטי כתוצאה ממטרת היעד של פריסת היישום script או win32 למשתמש/מכשיר.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="5f6e2-106">יש גם קבוצה של דרישות מוקדמות שיש לעמוד בהן כדי לפרוס אפליקציות Win32 הכוללות:</span><span class="sxs-lookup"><span data-stu-id="5f6e2-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="5f6e2-107">פלטפורמות נתמכות: Windows 10 גירסה 1607 ואילך (גירסאות Enterprise, Pro ו-השכלה).</span><span class="sxs-lookup"><span data-stu-id="5f6e2-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="5f6e2-108">ארכיטקטורה נתמכת: x86 ו-x64.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="5f6e2-109">ניהול מכשירים: הצטרף ל-עמ מ ונרשם באופן אוטומטי (כולל תחום היברידי המצורף ומדיניות קבוצתית שנרשמו באופן אוטומטי).</span><span class="sxs-lookup"><span data-stu-id="5f6e2-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="5f6e2-110">תבנית חבילת יישום:. קובץ **intunewin**  שהוכן על-ידי [כלי ההכנה של תוכן Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="5f6e2-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="5f6e2-111">מגבלות</span><span class="sxs-lookup"><span data-stu-id="5f6e2-111">Limitations:</span></span>
    - <span data-ttu-id="5f6e2-112">גודל מרבי: 8GB.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="5f6e2-113">ארכיטקטורה שאינה נתמכת: חימוש.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="5f6e2-114">סקור את הדוקטור "[הוסף, הקצה ונטר יישום Win32 ב-Microsoft intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" לקבלת מידע הקשור לשלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="5f6e2-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="5f6e2-115">פרטים אודות פתרון בעיות בפריסה של יישומים ב-Windows כולל יישומי Win32 ניתנים לסקירה במסמכים הבאים</span><span class="sxs-lookup"><span data-stu-id="5f6e2-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="5f6e2-116">פתרון בעיות בהתקנת יישומים</span><span class="sxs-lookup"><span data-stu-id="5f6e2-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="5f6e2-117">פתרון בעיות של יישומי Win32</span><span class="sxs-lookup"><span data-stu-id="5f6e2-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)