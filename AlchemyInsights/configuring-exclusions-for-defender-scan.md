---
title: קביעת התצורה של אי-הכללות עבור Microsoft Defender ATP סריקה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543686"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="98407-102">קביעת התצורה של אי-הכללות עבור Microsoft Defender ATP סריקה</span><span class="sxs-lookup"><span data-stu-id="98407-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="98407-103">באופן כללי, באפשרותך לא לכלול סיומות קבצים ומיקום תיקיה מסוימים Microsoft Defender ATP סריקות.</span><span class="sxs-lookup"><span data-stu-id="98407-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="98407-104">באפשרותך גם לקבוע תצורה של אי-הכללות עבור קבצים שנפתחו על-ידי תהליכים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="98407-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="98407-105">לקבלת מידע נוסף, ראה קביעת תצורה [ואמת של אי-הכללות בהתבסס](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) על סיומת קובץ ומיקום תיקיה והגדרה [של אי-הכללות עבור קבצים שנפתחו על-ידי תהליכים](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="98407-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="98407-106">כדי לקבוע תצורה של **אי-הכללות עבור Windows Server 2016 ו- 2019,** [ראה קביעת תצורה של אנטי-וירוס של Microsoft Defender אי-הכללות ב- Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="98407-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="98407-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="98407-107">**Mac**</span></span>

<span data-ttu-id="98407-108">לקבלת פרטים על סוגי אי-הכללה נתמכים וקביעת תצורה של רשימה של אי-הכללות עבור Mac, ראה סוגי [אי-הכללה](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) נתמכים ואופן קביעת התצורה [של רשימת אי-הכללות.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="98407-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="98407-109">**הערה** באפשרותך גם לאמת רשימות אי-הכללה באמצעות קובץ מחשב EICAR.</span><span class="sxs-lookup"><span data-stu-id="98407-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="98407-110">לקבלת מידע נוסף, ראה [אימות רשימות אי-הכללות עם קובץ מחשב של EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="98407-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="98407-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="98407-111">**Linux**</span></span>

<span data-ttu-id="98407-112">לקבלת פרטים על סוגי אי-הכללה נתמכים וקביעת התצורה של רשימה של אי-הכללות עבור Linux, ראה סוגי [אי-הכללה](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) נתמכים והגדרה של אי-הכללות [עבור Microsoft Defender ATP עבור Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="98407-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="98407-113">**הערה** באפשרותך גם לאמת רשימות אי-הכללה באמצעות קובץ מחשב EICAR.</span><span class="sxs-lookup"><span data-stu-id="98407-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="98407-114">לקבלת מידע נוסף, ראה [אימות רשימות אי-הכללות עם קובץ מחשב של EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="98407-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 