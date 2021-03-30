---
title: Troubleshoot Hybrid Azure AD join
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401908"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="eba8a-102">Troubleshoot Hybrid Azure AD join</span><span class="sxs-lookup"><span data-stu-id="eba8a-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="eba8a-103">מומלץ מאוד לוודא שמכשיר יכול לגשת לנקודות קצה לרישום מכשיר תחת חשבון המערכת באמצעות [קובץ ה- Script של בדיקת קישוריות רישום מכשיר](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="eba8a-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="eba8a-104">אם אתה מגדיר רישומי מכשירים בפעם הראשונה, הקפד לעיין ב[מבוא לניהול מכשירים ב- Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) כדי ללמוד כיצד לקבל מכשירים בשליטת Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eba8a-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="eba8a-105">אם אתה רושם מכשירים ל- Azure AD ישירות ורושם אותם ל- Intune, ודא תחילה ש[קבעת את התצורה של Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ושיש לך [רשיון](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="eba8a-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="eba8a-106">ודא שאתה מורשה לבצע פעולות ב- Azure AD וב- AD מקומי.</span><span class="sxs-lookup"><span data-stu-id="eba8a-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="eba8a-107">רק מנהל מערכת כללי ב- Azure AD יכול לנהל הגדרות עבור רישומי מכשירים.</span><span class="sxs-lookup"><span data-stu-id="eba8a-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="eba8a-108">בנוסף, אם אתה מגדיר רישומים אוטומטיים ב- Active Directory המקומי שלך, יהיה עליך להיות מנהל מערכת של Active Directory ו- AD FS (אם רלוונטי).</span><span class="sxs-lookup"><span data-stu-id="eba8a-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="eba8a-109">לקבלת פרטים נוספים על פתרון בעיות פוטנציאליות ב- Hybrid join, ראה [פתרון בעיות ב- Hybrid join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) עבור הגדרת משתמש ב- hybrid Azure AD join וניהול מכשירים באמצעות פורטל Azure Ad, ראה [הגדרת מכשירי משתמש ב- hybrid Azure AD join (מכשירי join של תחום מקומי)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ו[ניהול מכשירים באמצעות פורטל Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="eba8a-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="eba8a-110">כדי לפתור בעיות נפוצות ב- Hybrid Azure Active Directory (AD) join, ראה שאלות נפוצות על [שאלות נפוצות בנושאHybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="eba8a-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
