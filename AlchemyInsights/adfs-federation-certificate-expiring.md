---
title: פג תוקפם של אישור הפדרציה של ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737190"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="b7bcb-102">פג תוקפם של אישור הפדרציה של ADFS</span><span class="sxs-lookup"><span data-stu-id="b7bcb-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="b7bcb-103">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b7bcb-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="b7bcb-104">התקן את מודול מדריך ההפעלה התכלת של Microsoft עבור Windows PowerShell במחשב (אם המודול אינו מותקן כבר).</span><span class="sxs-lookup"><span data-stu-id="b7bcb-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="b7bcb-105">כדי לעשות זאת, ללכת [לנהל לספירה תכלת באמצעות Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="b7bcb-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="b7bcb-106">בצע את השלבים בסעיף "תרחיש 1: תוקף האישור של חתימת האסימון של AD FS" של ["אירעה בעיה בגישה לאתר" מתוך AD fs כאשר משתמש מאוחד מתחבר ל-Office 365, תכלת או Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="b7bcb-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="b7bcb-107">בצע את השלבים [בעדכון או תקן את ההגדרות של תחום מאוחד ב-Office 365, תכלת או Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="b7bcb-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="b7bcb-108">כדי ללמוד עוד אודות חידוש אישורי הפדרציה, ראה [חידוש אישורי הפדרציה עבור Office 365 ו-"כחול פעיל](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)".</span><span class="sxs-lookup"><span data-stu-id="b7bcb-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
