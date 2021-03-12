---
title: לא נמצאו הודעות מנויים במרכז האבטחה
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713604"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="9f44d-102">לא נמצאו הודעות מנויים במרכז האבטחה</span><span class="sxs-lookup"><span data-stu-id="9f44d-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="9f44d-103">אם בעת גישה למרכז האבטחה של Microsoft Defender, אתה מקבל את ההודעה "לא נמצאו מנויים", פירוש הדבר ש-תכלת Active Directory (עמ מ) המשמש לכניסה למשתמש לפורטל אינו כולל רשיון Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="9f44d-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="9f44d-104">רשיונות Windows E5 ו-Office E5 הם רשיונות נפרדים.</span><span class="sxs-lookup"><span data-stu-id="9f44d-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="9f44d-105">פתח את מקרה התמיכה אם הרשיון נרכש אך לא הוקצה למופע של הוראות התקנה.</span><span class="sxs-lookup"><span data-stu-id="9f44d-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="9f44d-106">יש לך:</span><span class="sxs-lookup"><span data-stu-id="9f44d-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="9f44d-107">בעיה אפשרית של הקצאת רשיונות.</span><span class="sxs-lookup"><span data-stu-id="9f44d-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="9f44d-108">בטעות הקצאת את הרשיון למספר משתמשים אחר של Microsoft מאשר האדם המשמש לאימות לשירות.</span><span class="sxs-lookup"><span data-stu-id="9f44d-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>