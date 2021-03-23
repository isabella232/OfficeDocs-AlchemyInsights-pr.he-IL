---
title: פתרון בעיות בקוד השגיאה AADSTS650056
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9803"
- "9005744"
ms.openlocfilehash: 945be2b496b98937bfae6d1f573162d1f2ebb4b6
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036650"
---
# <a name="troubleshoot-error-code-aadsts650056"></a><span data-ttu-id="18658-102">פתרון בעיות בקוד השגיאה AADSTS650056</span><span class="sxs-lookup"><span data-stu-id="18658-102">Troubleshoot error code AADSTS650056</span></span>

<span data-ttu-id="18658-103">כדי לפתור את השגיאה AADSTS650056, בצע את השלב המומלץ להלן.</span><span class="sxs-lookup"><span data-stu-id="18658-103">To resolve AADSTS650056 error, perform the below recommended step.</span></span>

<span data-ttu-id="18658-104">**AADSTS65005**: MisconfiguredApplication-רשימת הגישה למשאבים הנדרשת עבור היישום אינה מכילה יישומים הניתנים לאיתור על-ידי המשאב או יישום הלקוח ביקשו גישה למשאב, שלא צוין ברשימת הגישה למשאבים הדרושים או בשירות הגרף שהחזיר בקשה או משאב לא נמצא.</span><span class="sxs-lookup"><span data-stu-id="18658-104">**AADSTS65005**: MisconfiguredApplication - The app required resource access list does not contain apps discoverable by the resource or The client app has requested access to resource, which was not specified in its required resource access list or Graph service returned bad request or resource not found.</span></span> <span data-ttu-id="18658-105">אם היישום תומך ב-SAML, ייתכן שהגדרת את האפליקציה באמצעות מזהה שגוי (יישות).</span><span class="sxs-lookup"><span data-stu-id="18658-105">If the app supports SAML, you may have configured the app with the wrong Identifier (Entity).</span></span>

<span data-ttu-id="18658-106">לקבלת מידע נוסף, עיין במאמר פתרון בעיות עבור שגיאות [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app).</span><span class="sxs-lookup"><span data-stu-id="18658-106">For more information, see the troubleshooting article for error [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app).</span></span>
