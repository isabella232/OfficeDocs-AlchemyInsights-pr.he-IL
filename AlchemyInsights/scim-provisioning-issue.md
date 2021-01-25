---
title: בעיית הקצאת משאבים של SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949787"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="41f6f-102">בעיית הקצאת משאבים של SCIM</span><span class="sxs-lookup"><span data-stu-id="41f6f-102">SCIM provisioning issue</span></span>

<span data-ttu-id="41f6f-103">הקצאת משאבים אוטומטית מתייחסת ליצירת זהויות משתמשים ותפקידים ביישומי הענן שהמשתמשים זקוקים להם לגישה אליהם.</span><span class="sxs-lookup"><span data-stu-id="41f6f-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="41f6f-104">בנוסף ליצירת זהויות משתמשים, הקצאת משאבים אוטומטית כוללת את התחזוקה וההסרה של זהויות משתמשים כאשר מצב או תפקידים משתנים.</span><span class="sxs-lookup"><span data-stu-id="41f6f-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="41f6f-105">לפני שתתחיל בפריסה, באפשרותך לבדוק [כיצד](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) הקצאת המשאבים פועלת כדי ללמוד כיצד פועלת ההקצאה של תכלת active DIRECTORY (AD) וקבלת המלצות תצורה.</span><span class="sxs-lookup"><span data-stu-id="41f6f-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="41f6f-106">כמפתח יישומים, באפשרותך להשתמש במערכת עבור API של ניהול זהויות בין תחומים (SCIM) עבור ניהול משתמשים כדי לאפשר הקצאה אוטומטית של משתמשים וקבוצות בין היישום שלך לבין תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="41f6f-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="41f6f-107">[נקודת הקצה של BUILD SCIM וקביעת תצורה של הקצאת משאבים באמצעות מאמר תכלת לספירה](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) מתארת כיצד לבנות נקודת קצה של SCIM ולשלב אותה עם שירות הקצאת המשאבים של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="41f6f-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



