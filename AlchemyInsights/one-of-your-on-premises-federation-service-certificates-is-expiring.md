---
title: תוקפו של אחד מאישורי שירות האיחוד המקומיים שלך פג
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810053"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="f9305-102">תוקפו של אחד מאישורי שירות האיחוד המקומיים שלך פג</span><span class="sxs-lookup"><span data-stu-id="f9305-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="f9305-103">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="f9305-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="f9305-104">התקן את מודול Microsoft Azure Active Directory עבור Windows PowerShell במחשב (אם המודול עדיין לא מותקן).</span><span class="sxs-lookup"><span data-stu-id="f9305-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f9305-105">לשם כך, עבור אל [Azure Active Directory PowerShell עבור Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="f9305-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="f9305-106">בצע את השלבים בסעיף "תרחיש 1: פג תוקפו של אישור חתימת אסימון של AD FS" של שגיאת "אירעה בעיה בגישה לאתר" מ- AD FS כאשר משתמש מאוחד נכנס ל- [Microsoft 365 , Azure או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="f9305-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="f9305-107">בצע את השלבים המפורטים כיצד לעדכן או לתקן את ההגדרות של תחום מאוחד [ב- Microsoft 365 , Azure או Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="f9305-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="f9305-108">לקבלת מידע נוסף אודות חידוש אישורי איחוד, ראה חידוש [אישורים עבור O365 ו- Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="f9305-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

