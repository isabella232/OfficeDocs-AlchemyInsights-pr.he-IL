---
title: פתרון בעיות הצטרפות ל- Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405126"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="895fa-102">פתרון בעיות הצטרפות ל- Azure AD</span><span class="sxs-lookup"><span data-stu-id="895fa-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="895fa-103">אם אתה מגדיר רישומי מכשירים בפעם הראשונה, ודא שסתכלת על מבוא לניהול מכשירים ב- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) שינחה אותך כיצד להשיג מכשירים תחת השליטה ב- Azure AD.</span><span class="sxs-lookup"><span data-stu-id="895fa-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="895fa-104">אם אתה רושם מכשירים ל- Azure AD ישירות ורושם אותם ל- Intune, יהיה עליך לוודא שתצורת [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) נקבעה [והרשיון](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) יהיה במקום הראשון.</span><span class="sxs-lookup"><span data-stu-id="895fa-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="895fa-105">ודא שאתה מורשה לבצע פעולות ב- Azure AD.</span><span class="sxs-lookup"><span data-stu-id="895fa-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="895fa-106">רק מנהל מערכת כללי ב- Azure AD יכול לנהל הגדרות עבור רישומי מכשירים.</span><span class="sxs-lookup"><span data-stu-id="895fa-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="895fa-107">כדי לעשות את יישום ההצטרפות של Azure AD, ראה [תכנון Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="895fa-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="895fa-108">לקבלת פרטים נוספים על פתרון בעיות נפוצות בצירוף Azure AD, ראה שאלות נפוצות בנושא [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) ובמכשיר Windows 10 pro, ראה אין אפשרות להצטרף למכשיר Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) ל- Azure AD - צורך לשדרג ל- Microsoft Community</span><span class="sxs-lookup"><span data-stu-id="895fa-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
