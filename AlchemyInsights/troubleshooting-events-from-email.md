---
title: פתרון בעיות של אירועים מהדואר האלקטרוני
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658735"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="c9214-102">פתרון בעיות של אירועים מהדואר האלקטרוני</span><span class="sxs-lookup"><span data-stu-id="c9214-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="c9214-103">אימות שהתכונה זמינה עבור תיבת הדואר: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="c9214-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="c9214-104">לאחר מכן הסתכל על ' אירועים מדואר אלקטרוני ' **מייצא את הייצוא-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="c9214-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="c9214-105">ביומני ' אירועים מדואר אלקטרוני ', אתר את InternetMessageId שמתאים לפריט בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="c9214-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="c9214-106">TrustScore קובע אם הפריט נוסף או לא.</span><span class="sxs-lookup"><span data-stu-id="c9214-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="c9214-107">אירועים יתווספו רק אם TrustScore = "מהימן".</span><span class="sxs-lookup"><span data-stu-id="c9214-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="c9214-108">TrustScore נקבע על-ידי מאפייני SPF, Dkim או Dmarc, הנמצאים בכותרת ההודעה.</span><span class="sxs-lookup"><span data-stu-id="c9214-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="c9214-109">כדי להציג מאפיינים אלה:</span><span class="sxs-lookup"><span data-stu-id="c9214-109">To view these properties:</span></span>

<span data-ttu-id="c9214-110">**Outlook בשולחן העבודה**</span><span class="sxs-lookup"><span data-stu-id="c9214-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="c9214-111">פתיחת הפריט</span><span class="sxs-lookup"><span data-stu-id="c9214-111">Open the item</span></span>
- <span data-ttu-id="c9214-112">מאפייני קובץ->-כותרות אינטרנט של ></span><span class="sxs-lookup"><span data-stu-id="c9214-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="c9214-113">או</span><span class="sxs-lookup"><span data-stu-id="c9214-113">or</span></span>

<span data-ttu-id="c9214-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="c9214-114">**MFCMapi**</span></span>

- <span data-ttu-id="c9214-115">ניווט לפריט בתיבת הדואר הנכנס</span><span class="sxs-lookup"><span data-stu-id="c9214-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="c9214-116">חפש PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="c9214-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="c9214-117">מאפיינים אלה נקבעים ומוקלטים במהלך ההעברה והניתוב.</span><span class="sxs-lookup"><span data-stu-id="c9214-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="c9214-118">לקבלת פתרון בעיות נוסף, ייתכן שתצטרך להמשיך בטיפול בתמיכה בנושאי תעבורה לגבי הכשלים ב-SPF, DKIM ו-. or DMARC.</span><span class="sxs-lookup"><span data-stu-id="c9214-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>