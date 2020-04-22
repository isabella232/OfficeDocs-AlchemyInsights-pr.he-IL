---
title: זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716425"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="0eaa5-102">זיהוי פעילות כלל תיבת דואר נכנס ביומני ביקורת</span><span class="sxs-lookup"><span data-stu-id="0eaa5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="0eaa5-103">באפשרותך להשתמש בחיפוש ביומן הביקורת ב-Microsoft 365 Security _ מרכז התאימות של מיקרוסופט כדי להציג אירועים של כלל תיבת דואר נכנס (יצירה, שינוי ומחיקה של כללי תיבת דואר נכנס).</span><span class="sxs-lookup"><span data-stu-id="0eaa5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="0eaa5-104">היכנס ל- [Microsoft 365 האבטחה _ אמפר _ מרכז התאימות](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0eaa5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0eaa5-105">עבור אל דף **Search** > **החיפוש של יומן ביקורת** חיפוש.</span><span class="sxs-lookup"><span data-stu-id="0eaa5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="0eaa5-106">בחר את טווח התאריכים **בתאריך ההתחלה** ושדות **הסיום** .</span><span class="sxs-lookup"><span data-stu-id="0eaa5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="0eaa5-107">תחת **החלפת פעילויות תיבת דואר**, ודא שהשדה **פעילויות** מוגדר **לחדש-inboxrule יצירה/שינוי/הפעלה/השבתה של כלל תיבת דואר נכנס**.</span><span class="sxs-lookup"><span data-stu-id="0eaa5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="0eaa5-108">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="0eaa5-108">Click **Search**.</span></span>

<span data-ttu-id="0eaa5-109">בתוצאות, בחר ברשומת ביקורת.</span><span class="sxs-lookup"><span data-stu-id="0eaa5-109">In the results, select an audit record.</span></span> <span data-ttu-id="0eaa5-110">בתפריט הפרטי, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="0eaa5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="0eaa5-111">מידע אודות הגדרות כלל תיבת הדואר הנכנס מוצג בשדה **Parameters** .</span><span class="sxs-lookup"><span data-stu-id="0eaa5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="0eaa5-112">לקבלת מידע נוסף, ראה [קביעה אם משתמש יצר כלל תיבת דואר נכנס](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="0eaa5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
