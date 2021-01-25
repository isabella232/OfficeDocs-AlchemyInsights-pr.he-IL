---
title: מיפוי תכונות של הקצאת משתמשים
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
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949763"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="b7faf-102">מיפוי תכונות של הקצאת משתמשים</span><span class="sxs-lookup"><span data-stu-id="b7faf-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="b7faf-103">כדי לפתור בעיות ידועות במיפוי התכונות, ראה [מיפויי תכונות](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="b7faf-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="b7faf-104">Microsoft תכלת Active Directory (AD) מספק תמיכה עבור הקצאת משתמשים ליישומי SaaS של ספקים חיצוניים כגון Salesforce, G Suite ואחרים.</span><span class="sxs-lookup"><span data-stu-id="b7faf-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="b7faf-105">אם אתה מאפשר הקצאת משאבים עבור יישום של SaaS של ספק חיצוני, פורטל התכלת קובע את ערכי התכונות שלו באמצעות מיפויי תכונות.</span><span class="sxs-lookup"><span data-stu-id="b7faf-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="b7faf-106">כדי ללמוד כיצד להתאים אישית את התכונה המוגדרת כברירת מחדל-מיפויים, ראה [התאמה אישית של תכונת הקצאת משתמשים-מיפויים עבור יישומי SaaS ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="b7faf-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="b7faf-107">לקבלת מידע נוסף אודות הקצאת משאבים של SaaS app, ראה [מהי הקצאת משתמשים אוטומטית של saas app בתכלת לספירה?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="b7faf-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="b7faf-108">בעת התאמה אישית של תכונה-מיפויים עבור הקצאת משאבים, ייתכן שתגלה שהתכונה שברצונך למפות אינה מופיעה ברשימה תכונת המקור.</span><span class="sxs-lookup"><span data-stu-id="b7faf-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="b7faf-109">[סינכרון תכונה ממדריך הכתובות המקומי של Active Directory לכיוון תכלת ad לצורך הקצאת מאמר ליישום](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) מראה לך כיצד להוסיף את התכונה החסרה על-ידי סינכרון מהמודעה המקומית שלך ל-תכלת ad.</span><span class="sxs-lookup"><span data-stu-id="b7faf-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
