---
title: ProxyAddress שגוי
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
ms.custom: ''
ms.assetid: c4cea778-1b26-4aea-bde8-4b7605e35886
ms.openlocfilehash: e0552b9d4ba1beeda14f6a46773060aede43e928
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801509"
---
# <a name="proxyaddress-incorrect"></a><span data-ttu-id="e1345-102">ProxyAddress שגוי</span><span class="sxs-lookup"><span data-stu-id="e1345-102">ProxyAddress incorrect</span></span>

<span data-ttu-id="e1345-103">כאשר אובייקט מסתנכרן עם תכלת לספירה, הערכים המצוינים בתכונה proxyAddresses ב-Active Directory מושווים לכללי הפרסום של התכלת ולאחר מכן התכונה proxyAddresses מאוכלסת ב-תכלת AD.</span><span class="sxs-lookup"><span data-stu-id="e1345-103">When an object is synchronized to Azure AD, the values that are specified in the proxyAddresses attribute in Active Directory are compared with Azure AD rules, and then the proxyAddresses attribute is populated in Azure AD.</span></span> <span data-ttu-id="e1345-104">לכן, ייתכן שהערכים של התכונה proxyAddresses עבור האובייקט ב-Active Directory אינם זהים לערכים של התכונה proxyAddresses בתכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="e1345-104">Therefore, the values of the proxyAddresses attribute for the object in Active Directory may not be the same as the values of the proxyAddresses attribute in Azure AD.</span></span>
  
<span data-ttu-id="e1345-105">לקבלת מידע נוסף על אופן האכלוס של proxyaddress, ראה [כיצד התכונה proxyaddress מאוכלסת בתכלת לספירה](https://support.microsoft.com/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="e1345-105">To learn more about how the proxyaddress is populated, see [How the proxyAddress attribute is populated in Azure AD](https://support.microsoft.com/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span></span>
  

