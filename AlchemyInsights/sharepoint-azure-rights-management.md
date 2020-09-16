---
title: הגבל גישה ב-SharePoint או ב-OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: cc6f93ba8ae3a030f83da5eca2d28dcf38f0f8f7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800897"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="3ac7c-102">הגנה באמצעות IRM על קבצי SharePoint</span><span class="sxs-lookup"><span data-stu-id="3ac7c-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="3ac7c-103">בתוך SharePoint Online, הגנת IRM מוחלת על קבצים ברמת הרשימה והספריה.</span><span class="sxs-lookup"><span data-stu-id="3ac7c-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="3ac7c-104">לפני שהארגון שלך יכול להשתמש בהגנת IRM, עליך להגדיר תחילה ניהול זכויות.</span><span class="sxs-lookup"><span data-stu-id="3ac7c-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="3ac7c-105">IRM מסתמך על שירות הניהול של זכויות תכלת מתוך הגנה על מידע תכלת כדי להצפין ולהקצות הגבלות שימוש.</span><span class="sxs-lookup"><span data-stu-id="3ac7c-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="3ac7c-106">מנויי Microsoft 365 מסוימים כוללים את ניהול זכויות התכלת, אך לא את כולם.</span><span class="sxs-lookup"><span data-stu-id="3ac7c-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="3ac7c-107">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="3ac7c-107">To learn more, see:</span></span>

- <span data-ttu-id="3ac7c-108">[כיצד יישומים ושירותים של Office תומכים בניהול זכויות של תכלת](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span><span class="sxs-lookup"><span data-stu-id="3ac7c-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="3ac7c-109">[הגדרת ניהול זכויות מידע (IRM) במרכז הניהול של SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span><span class="sxs-lookup"><span data-stu-id="3ac7c-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="3ac7c-110">[IRM-הפיכת ספריות מסמכים ורשימות של SharePoint לזמינות](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span><span class="sxs-lookup"><span data-stu-id="3ac7c-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="3ac7c-111">[ניהול זכויות מידע ב-Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span><span class="sxs-lookup"><span data-stu-id="3ac7c-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="3ac7c-112">[ניהול זכויות מידע ב-Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="3ac7c-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>


