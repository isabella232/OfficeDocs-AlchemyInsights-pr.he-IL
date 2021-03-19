---
title: אישור האיחוד של ADFS עומד לפוג
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686715"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="2ee9f-102">אישור האיחוד של ADFS עומד לפוג</span><span class="sxs-lookup"><span data-stu-id="2ee9f-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="2ee9f-103">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2ee9f-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="2ee9f-104">התקן את מודול Microsoft של Active Directory עבור Windows PowerShell במחשב (אם המודול אינו מותקן עדיין).</span><span class="sxs-lookup"><span data-stu-id="2ee9f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="2ee9f-105">לשם כך, עבור אל [ניהול AD תכולים באמצעות Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="2ee9f-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="2ee9f-106">בצע את השלבים המפורטים בסעיף "תרחיש 1: תוקף אישור האסימון לחתימה של AD FS" של ["אירעה בעיה בגישה לאתר" מתוך AD FS כאשר משתמש מאוחד נכנס ל-Microsoft 365, לתכלת או למנגינה](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="2ee9f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="2ee9f-107">בצע את השלבים המפורטים [בעדכון או תיקון ההגדרות של תחום מאוחד ב-Microsoft, בתכלת או במנגינה](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="2ee9f-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="2ee9f-108">לקבלת מידע נוסף על חידוש אישורי איחוד, ראה [חידוש אישורי איחוד עבור Microsoft 365 ו-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="2ee9f-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
