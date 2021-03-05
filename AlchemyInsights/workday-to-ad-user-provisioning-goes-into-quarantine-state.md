---
title: יום עבודה לפרסום הקצאת משתמשים נכנסת למצב הסגר
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481875"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="d60c8-102">יום עבודה לפרסום הקצאת משתמשים נכנסת למצב הסגר</span><span class="sxs-lookup"><span data-stu-id="d60c8-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="d60c8-103">**יום עבודה כדי להעביר הקצאת משתמשים נכנסת למצב הסגר ולא נוצרות משתמשים ב-AD**</span><span class="sxs-lookup"><span data-stu-id="d60c8-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="d60c8-104">משימת הקצאת המשאבים למשתמש של יום העבודה עברה למצב ההסגר ויומני הביקורת מראים אירועי כשל ייצוא עם שגיאת הודעת השגיאה **: OperationsError-SvcErr: אירעה שגיאת פעולה. לא הוגדרו הפניה מעולה עבור שירות מדריך הכתובות. לפיכך, שירות מדריך הכתובות אינו מצליח להנפיק הפניות לאובייקטים מחוץ ליער זה**.</span><span class="sxs-lookup"><span data-stu-id="d60c8-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="d60c8-105">שגיאה זו בדרך כלל מופיעה אם הגורם המכיל של Active Directory אינו מוגדר כהלכה או אם קיימות בעיות במיפוי הביטויים המשמש **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="d60c8-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="d60c8-106">סמן את הפרמטר OU המוגדר כברירת מחדל עבור **משתמשים חדשים** עבור הקלדה.</span><span class="sxs-lookup"><span data-stu-id="d60c8-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="d60c8-107">ודא שה-OU שצוין כבר קיים במודעה שלך.</span><span class="sxs-lookup"><span data-stu-id="d60c8-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="d60c8-108">אם אתה משתמש ב- **parentDistinguishedName** במיפוי התכונות, ודא שהוא תמיד מוערך כגורם מכיל מוכר בתוך התחום המודע.</span><span class="sxs-lookup"><span data-stu-id="d60c8-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="d60c8-109">סמן את אירוע הייצוא ביומני הביקורת כדי לראות את הערך שנוצר.</span><span class="sxs-lookup"><span data-stu-id="d60c8-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="d60c8-110">לקבלת פרטים נוספים על קביעת התצורה של יום העבודה לצורך הקצאה אוטומטית, ראה [ערכת לימוד: קביעת התצורה של יום עבודה עבור הקצאת משתמשים אוטומטית](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="d60c8-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

