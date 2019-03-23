---
title: אחד מהאישורים השירות שלך הפדרציה המקומית תאריך תפוגה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753031"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="eaff6-102">אחד מהאישורים השירות שלך הפדרציה המקומית תאריך תפוגה</span><span class="sxs-lookup"><span data-stu-id="eaff6-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="eaff6-103">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="eaff6-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="eaff6-104">התקן את Microsoft תכלת הרקיע Active Directory מודול עבור Windows PowerShell במחשב (אם המודול אינו מותקן כבר).</span><span class="sxs-lookup"><span data-stu-id="eaff6-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="eaff6-105">כדי לעשות זאת, עבור אל [תכלת הרקיע Active Directory PowerShell עבור גרף](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="eaff6-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="eaff6-106">בצע את השלבים ב "תרחיש 1: פג תוקפו של האישור חתימת אסימון AD FS" מקטע של [השגיאה "אירעה בעיה בגישה אל האתר" מתוך AD FS כאשר משתמש מאוחד יוסיף ב- Office 365, תכלת הרקיע, או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="eaff6-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="eaff6-107">בצע את השלבים ב- t[כיצד לעדכן או לתקן את ההגדרות של תחום מאוחד ב- Office 365, תכלת הרקיע, או Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="eaff6-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="eaff6-108">לקבלת מידע נוסף אודות חידוש אישורים הפדרציה, ראה [חידוש האישור עבור O365 ו- AD תכלת הרקיע](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="eaff6-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

