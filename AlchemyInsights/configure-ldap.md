---
title: קביעת התצורה של LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885161"
---
# <a name="configure-ldap"></a><span data-ttu-id="ab864-102">קביעת התצורה של LDAP</span><span class="sxs-lookup"><span data-stu-id="ab864-102">Configure LDAP</span></span>

<span data-ttu-id="ab864-103">כדי לקבוע את תצורת LDAP, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ab864-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="ab864-104">בדוק את תקינות התחום שלך [בפורטל התכלת](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="ab864-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="ab864-105">ודא שמנוי חוקי של תכלת לספירה זמין ושירותי התחום של תכלת AD הופעלו.</span><span class="sxs-lookup"><span data-stu-id="ab864-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="ab864-106">יש לקבל את האישור הנדרש להפיכת LDAP מאובטחת מרשות אישורים ציבורית מהימנה או להיות אישור בחתימה עצמית.</span><span class="sxs-lookup"><span data-stu-id="ab864-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="ab864-107">ודא שהאישור עוקב אחר [הקווים המנחים](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)הדרושים.</span><span class="sxs-lookup"><span data-stu-id="ab864-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="ab864-108">**אישור לא חוקי**</span><span class="sxs-lookup"><span data-stu-id="ab864-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="ab864-109">כדי לחדש אישור, בצע את השלבים ליצירת אישור חדש והעלאה מחדש: [קביעת התצורה של LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ab864-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="ab864-110">כדי לפתור בעיה ידועה באמצעות התראות LDAP מאובטחות בשירותי התחום של Active directory, ראה [פתרון התראות של ldap](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ab864-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
