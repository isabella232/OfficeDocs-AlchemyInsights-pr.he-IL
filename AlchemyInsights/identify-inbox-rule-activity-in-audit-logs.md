---
title: זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417248"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="66171-102">זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת</span><span class="sxs-lookup"><span data-stu-id="66171-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="66171-103">באפשרותך להשתמש בחיפוש יומן ביקורת ב- & אבטחה מרכז תאימות כדי להציג אירועים כלל תיבת דואר נכנס (יצירה, שינוי ומחיקה של כללי תיבת דואר נכנס).</span><span class="sxs-lookup"><span data-stu-id="66171-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="66171-104">היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="66171-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="66171-105">לחץ על **חיפוש ויצירת החקירה** ובחר באפשרות **החיפוש יומן ביקורת**.</span><span class="sxs-lookup"><span data-stu-id="66171-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="66171-106">בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** .</span><span class="sxs-lookup"><span data-stu-id="66171-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="66171-107">תחת **הפעילויות תיבת הדואר של Exchange**, ודא **פעילויות** שהשדה מוגדר **InboxRule חדש צור/לשנות/הפעל/בטל כלל תיבת דואר נכנס**.</span><span class="sxs-lookup"><span data-stu-id="66171-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="66171-108">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="66171-108">Click **Search**.</span></span>

<span data-ttu-id="66171-109">בתוצאות, בחר את רשומת הביקורת.</span><span class="sxs-lookup"><span data-stu-id="66171-109">In the results, select an audit record.</span></span> <span data-ttu-id="66171-110">תפריט נשלף של פרטים, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="66171-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="66171-111">מידע אודות הגדרות הכלל בתיבת הדואר הנכנס מוצג בשדה **פרמטרים** .</span><span class="sxs-lookup"><span data-stu-id="66171-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="66171-112">לקבלת מידע נוסף, ראה [קביעת אם משתמש נוצר כלל תיבת הדואר הנכנס](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="66171-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
