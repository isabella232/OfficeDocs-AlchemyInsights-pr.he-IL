---
title: בעיות סודיות של לקוח רישום אפליקציה או אישורים
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404787"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="4ba2d-102">בעיות סודיות של לקוח רישום אפליקציה או אישורים</span><span class="sxs-lookup"><span data-stu-id="4ba2d-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="4ba2d-103">פג תוקפו של לקוח יישום סודי?</span><span class="sxs-lookup"><span data-stu-id="4ba2d-103">Application client secret expiring?</span></span>

<span data-ttu-id="4ba2d-104">ללא קשר לאופן יצירת היישום הרשום, בין אם באמצעות תהליך הרישום הרגיל בפורטל רישום היישומים או אם מנהל השירות נוצר הדייר שלך באמצעות הסכמת היישום, יש ליצור סוד לקוח חדש לפני התפוגה של היישום הנוכחי ולעדכן אותו בקוד היישום הקשור.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="4ba2d-105">תקופת התוקף המרבית היא שנתיים.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="4ba2d-106">כתזכורת, יש להקליט את הערך הסודי, כי הוא לא יהיה גלוי עוד לאחר שהוא עוזב את הדף 'רישומי אפליקציה' בפורטל.</span><span class="sxs-lookup"><span data-stu-id="4ba2d-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="4ba2d-107">לקבלת מידע נוסף, ראה [התחלה מהירה: רישום יישום בפלטפורמות הזהויות](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) של Microsoft ושיטות [עבודה מומלצות עבור פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="4ba2d-108">כדי ללמוד עוד, ראה [יצירת יישום Azure AD & השירות הראשי בפורטל - פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="4ba2d-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
