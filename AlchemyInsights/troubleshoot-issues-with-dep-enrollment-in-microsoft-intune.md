---
title: פתרון בעיות בהרשמת DEP ב-Microsoft intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797297"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="d919a-102">פתרון בעיות בהרשמת DEP ב-Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="d919a-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="d919a-103">סקור את המשאבים המפורטים להלן כדי לפתור את הבעיה כעת.</span><span class="sxs-lookup"><span data-stu-id="d919a-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="d919a-104">אם להתקן DEP אין אפשרות להירשם ולתואר שאינו מקומי (אימות רב-גורמי) זמין, בטל את התכונה ' ביטול תואר שולי '.</span><span class="sxs-lookup"><span data-stu-id="d919a-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="d919a-105">בשלב זה, משרד החוץ אינו נתמך עבור הרשמת DEP</span><span class="sxs-lookup"><span data-stu-id="d919a-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="d919a-106">השתמש [בפורטל לפתרון בעיות](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) ב-intune כדי לאבחן ולפתור כשלונות הרשמה נפוצים.</span><span class="sxs-lookup"><span data-stu-id="d919a-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d919a-107">סקור [מסמך זה](https://docs.microsoft.com/intune/help-desk-operators) לקבלת פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="d919a-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="d919a-108">סקור מסמכים אלה לקבלת רשימה של שגיאות נפוצות המונעות הרשמה ורזולוציות לכל אחת מהן: [מדריך לפתרון בעיות ומדריך](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [לפתרון בעיות](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="d919a-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="d919a-109">[למד אודות התוכנית להרשמת מכשירים](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="d919a-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
