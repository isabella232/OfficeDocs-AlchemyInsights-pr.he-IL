---
title: זיהוי כתובת IP ולקוח ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508917"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="1a695-102">זיהוי כתובת IP ולקוח ביומני ביקורת</span><span class="sxs-lookup"><span data-stu-id="1a695-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="1a695-103">כתובת ה-IP התואמת לפעילות על-ידי משתמש של Microsoft 365 או מנהל מערכת מוצגת ביומני ביקורת.</span><span class="sxs-lookup"><span data-stu-id="1a695-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="1a695-104">מידע הלקוח נרשם גם הוא.</span><span class="sxs-lookup"><span data-stu-id="1a695-104">The client information is also logged.</span></span> <span data-ttu-id="1a695-105">להלן השלבים לזיהוי מידע שכזה</span><span class="sxs-lookup"><span data-stu-id="1a695-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="1a695-106">היכנס ל- [Microsoft 365 האבטחה _ אמפר _ מרכז התאימות](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1a695-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="1a695-107">עבור אל דף **Search**  >  **החיפוש של יומן ביקורת** החיפוש.</span><span class="sxs-lookup"><span data-stu-id="1a695-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="1a695-108">אם אתה מעוניין בפעילות מסוימת, בחר אותה מתוך רשימת **הפעילויות** .</span><span class="sxs-lookup"><span data-stu-id="1a695-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="1a695-109">אם לא, כל הפעילויות יוחזרו עבור המשתמש הנבחר (הגדרת ברירת המחדל).</span><span class="sxs-lookup"><span data-stu-id="1a695-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="1a695-110">**הערה**: ייתכן שפעילויות מסוימות לא יהיו זמינות בתפריט ' **פעילויות** '; עם זאת, פריטי ביקורת אלה יוחזרו אם האפשרות **הצג תוצאות עבור כל הפעילויות** נבחרה (הגדרת ברירת המחדל).</span><span class="sxs-lookup"><span data-stu-id="1a695-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="1a695-111">ציין את שם המשתמש בשדה **Users** , בחר את טווח התאריכים המתאים עבור הפעילות ולאחר מכן לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="1a695-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="1a695-112">בתוצאות, באפשרותך לראות את כתובת ה-IP עבור פעילות זו בחלונית התוצאות.</span><span class="sxs-lookup"><span data-stu-id="1a695-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="1a695-113">בחר ברשומת הביקורת כדי לראות מידע מפורט בתפריט **הפרטים** (לדוגמה, לקוח, משתמש שביצע פעולה וכו ').</span><span class="sxs-lookup"><span data-stu-id="1a695-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="1a695-114">לקבלת מידע נוסף, ראה [איתור כתובת ה-IP של המחשב המשמש לקבלת גישה לחשבון שנפרץ](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="1a695-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
