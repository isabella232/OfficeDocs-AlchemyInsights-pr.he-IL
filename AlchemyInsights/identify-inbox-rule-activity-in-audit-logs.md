---
title: זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755039"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="c023f-102">זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת</span><span class="sxs-lookup"><span data-stu-id="c023f-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="c023f-103">באפשרותך להשתמש בחיפוש יומן ביקורת ב- & אבטחה מרכז תאימות כדי להציג אירועים כלל תיבת דואר נכנס (יצירה, שינוי ומחיקה של כללי תיבת דואר נכנס).</span><span class="sxs-lookup"><span data-stu-id="c023f-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="c023f-104">היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c023f-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c023f-105">לחץ על **חיפוש ויצירת החקירה** ובחר באפשרות **החיפוש יומן ביקורת**.</span><span class="sxs-lookup"><span data-stu-id="c023f-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c023f-106">בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** .</span><span class="sxs-lookup"><span data-stu-id="c023f-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="c023f-107">תחת **הפעילויות תיבת הדואר של Exchange**, ודא **פעילויות** שהשדה מוגדר **InboxRule חדש צור/לשנות/הפעל/בטל כלל תיבת דואר נכנס**.</span><span class="sxs-lookup"><span data-stu-id="c023f-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="c023f-108">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="c023f-108">Click **Search**.</span></span>

<span data-ttu-id="c023f-109">בתוצאות, בחר את רשומת הביקורת.</span><span class="sxs-lookup"><span data-stu-id="c023f-109">In the results, select an audit record.</span></span> <span data-ttu-id="c023f-110">תפריט נשלף של פרטים, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="c023f-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c023f-111">מידע אודות הגדרות הכלל בתיבת הדואר הנכנס מוצג בשדה **פרמטרים** .</span><span class="sxs-lookup"><span data-stu-id="c023f-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="c023f-112">לקבלת מידע נוסף, ראה [קביעת אם משתמש נוצר כלל תיבת הדואר הנכנס](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="c023f-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
