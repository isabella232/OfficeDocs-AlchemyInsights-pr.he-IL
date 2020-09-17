---
title: זיהוי פעילות כלל של תיבת דואר נכנס ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779052"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="607f5-102">זיהוי פעילות כלל של תיבת דואר נכנס ביומני ביקורת</span><span class="sxs-lookup"><span data-stu-id="607f5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="607f5-103">באפשרותך להשתמש בחיפוש ביומן הביקורת במרכז התאימות של Microsoft 365 Security & כדי להציג אירועים של כללי תיבת דואר נכנס (יצירה, שינוי ומחיקה של כללי תיבת דואר נכנס).</span><span class="sxs-lookup"><span data-stu-id="607f5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="607f5-104">היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="607f5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="607f5-105">עבור אל דף **Search**  >  **החיפוש ביומן ביקורת** חיפוש.</span><span class="sxs-lookup"><span data-stu-id="607f5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="607f5-106">בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך סיום** .</span><span class="sxs-lookup"><span data-stu-id="607f5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="607f5-107">תחת **פעילויות של תיבת דואר של Exchange**, ודא שהשדה ' **פעילויות** ' מוגדר ל **-New-InboxRule יצירה/שינוי/הפעלה/ביטול של כלל תיבת דואר נכנס**.</span><span class="sxs-lookup"><span data-stu-id="607f5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="607f5-108">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="607f5-108">Click **Search**.</span></span>

<span data-ttu-id="607f5-109">בתוצאות, בחר רשומת ביקורת.</span><span class="sxs-lookup"><span data-stu-id="607f5-109">In the results, select an audit record.</span></span> <span data-ttu-id="607f5-110">בנשלף של הפרטים, לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="607f5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="607f5-111">מידע אודות הגדרות הכלל של תיבת הדואר הנכנס מוצג בשדה **פרמטרים** .</span><span class="sxs-lookup"><span data-stu-id="607f5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="607f5-112">לקבלת מידע נוסף, ראה [קביעה אם משתמש יצר כלל תיבת דואר נכנס](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="607f5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
