---
title: 'שגיאה: הכללים במחשב זה אינם תואמים'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690964"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="dab33-102">שגיאה: הכללים במחשב זה אינם תואמים</span><span class="sxs-lookup"><span data-stu-id="dab33-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="dab33-103">כדי לראות את המצב המעודכן של בעיה ידועה זו, ראה [הכללים במחשב זה אינם תואמים לכללים ב-Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="dab33-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="dab33-104">צוות Outlook יישם תיקון בגירסת Build מס ' 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="dab33-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="dab33-105">התיקון נמצא כבר במהירות מיקומית והוא יעבור לערוץ החודשי בסוף יוני 2020.</span><span class="sxs-lookup"><span data-stu-id="dab33-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="dab33-106">לאחר שבנית את גירסת ה-build הקבועה, אתה עשוי לקבל את הבקשה "אילו כללים ברצונך להשאיר" בפעם האחרונה.</span><span class="sxs-lookup"><span data-stu-id="dab33-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="dab33-107">בחר שרת כאשר תתבקש לעשות זאת ולאחר מכן חזור ל-Outlook והפעל מחדש את הכללים שהפכו ללא זמינים.</span><span class="sxs-lookup"><span data-stu-id="dab33-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="dab33-108">עד שהתיקון יהיה זמין, השתמש בפתרון הבא:</span><span class="sxs-lookup"><span data-stu-id="dab33-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="dab33-109">**פתרון**: בדוחות אחרונים, אירעה הבעיה עבור אלה שיצרו רק כללי לקוח בשולחן העבודה של Outlook.</span><span class="sxs-lookup"><span data-stu-id="dab33-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="dab33-110">אם אתה ממשיך להיתקל בבעיה, שקול למחוק את הכללים ולאחר מכן ליצור ולערוך כללים רק ב-OWA (Outlook Web App) עד לפתרון הבעיה.</span><span class="sxs-lookup"><span data-stu-id="dab33-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="dab33-111">אם אין באפשרותך למחוק את הכללים באופן ידני, באפשרותך להפעיל פקודת Outlook כאשר אתה מפעיל את Outlook על-ידי הפעלת Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="dab33-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="dab33-112">פעולה זו תגרום למחיקת כללי הלקוח והשרת.</span><span class="sxs-lookup"><span data-stu-id="dab33-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="dab33-113">הוא ימחק את כל הכללים עבור כל החשבונות בפרופיל Outlook.</span><span class="sxs-lookup"><span data-stu-id="dab33-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="dab33-114">פקודה זו מתועדת עוד יותר במאמר בוררי שורת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="dab33-114">This command is further documented in the Command-line switches article.</span></span>

