---
title: לא נמצאו הודעות של מנויים במרכז האבטחה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544109"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="1ee40-102">לא נמצאו הודעות של מנויים במרכז האבטחה</span><span class="sxs-lookup"><span data-stu-id="1ee40-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="1ee40-103">אם בעת הגישה מרכז האבטחה של Microsoft Defender אתה מקבל הודעת "לא נמצאו מנויים", פירוש הדבר ש- Azure Active Directory (AAD) המשמש כדי להיכנס למשתמש לפורטל אינו כולל רשיון Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="1ee40-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="1ee40-104">הרשיונות Windows E5 Office E5 הם רשיונות נפרדים.</span><span class="sxs-lookup"><span data-stu-id="1ee40-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="1ee40-105">פתח מקרה תמיכה אם הרשיון נרכש אך לא הוקצה למופע AAD זה.</span><span class="sxs-lookup"><span data-stu-id="1ee40-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="1ee40-106">או שיש לך:</span><span class="sxs-lookup"><span data-stu-id="1ee40-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="1ee40-107">בעיה אפשרית בהקצאת רשיון.</span><span class="sxs-lookup"><span data-stu-id="1ee40-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="1ee40-108">הקצאת בטעות את הרשיון ל- AAD אחר של Microsoft מזה ששימש לאימות בשירות.</span><span class="sxs-lookup"><span data-stu-id="1ee40-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>