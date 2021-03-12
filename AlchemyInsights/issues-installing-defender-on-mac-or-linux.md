---
title: בעיות בהתקנת Microsoft Defender ב-Mac או ב-Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713544"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="9e517-102">בעיות בהתקנת Microsoft Defender ב-Mac או ב-Linux</span><span class="sxs-lookup"><span data-stu-id="9e517-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="9e517-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="9e517-103">**Mac**</span></span>

- <span data-ttu-id="9e517-104">ודא שדרישות המערכת נפגשות לפני התקנת Microsoft Defender ATP עבור Mac.</span><span class="sxs-lookup"><span data-stu-id="9e517-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="9e517-105">לקבלת מידע נוסף, ראה [כיצד להתקין את Microsoft DEFENDER ATP עבור Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="9e517-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="9e517-106">סקור את המידע בקובץ: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="9e517-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="9e517-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="9e517-107">**Linux**</span></span>

- <span data-ttu-id="9e517-108">ודא שדרישות המערכת נפגשות לפני התקנת Microsoft Defender ATP עבור Linux.</span><span class="sxs-lookup"><span data-stu-id="9e517-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="9e517-109">לקבלת מידע נוסף, ראה [כיצד להתקין את Microsoft DEFENDER ATP עבור Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="9e517-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="9e517-110">כדי לוודא ששירות MDATP פועל, ראה [ההתקנה נכשלה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="9e517-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="9e517-111">כדי לפתור בעיות ולפתור בעיות אם השירות אינו פועל, ראה [שלבים לפתרון בעיות אם השירות של mdatp אינו פועל](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="9e517-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="9e517-112">לקבלת שלבים לבדיקת תצורת הלקוח, המאמתת את תקינות המוצר ולהפעלת בדיקת זיהוי בקובץ הטקסט של EICAR, ראה [תצורת לקוח](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="9e517-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="9e517-113">**הערה** לקבלת רשימה של מערכות קבצים נתמכות עבור פעילות בגישה, ראה [Microsoft DEFENDER ATP עבור Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="9e517-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>