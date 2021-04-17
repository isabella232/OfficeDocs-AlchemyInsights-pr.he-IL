---
title: פתרון בעיות של אירועים מתוך דואר אלקטרוני
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834840"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="58b71-102">פתרון בעיות של אירועים מתוך דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="58b71-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="58b71-103">ודא שהתכונה זמינה עבור תיבת הדואר: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="58b71-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="58b71-104">לאחר מכן, הבט ביומני 'אירועים בדואר אלקטרוני' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="58b71-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="58b71-105">ביומני הרישום של 'אירועים בדואר אלקטרוני', חפש את InternetMessageId התואם לפריט בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="58b71-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="58b71-106">TrustScore קובע אם הפריט נוסף או לא.</span><span class="sxs-lookup"><span data-stu-id="58b71-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="58b71-107">אירועים יתווספו רק אם TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="58b71-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="58b71-108">TrustScore נקבע על-ידי מאפייני SPF, Dkim או Dmarc, הנמצאים בכותרת ההודעה.</span><span class="sxs-lookup"><span data-stu-id="58b71-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="58b71-109">כדי להציג מאפיינים אלה:</span><span class="sxs-lookup"><span data-stu-id="58b71-109">To view these properties:</span></span>

<span data-ttu-id="58b71-110">**Outlook לשולחן העבודה**</span><span class="sxs-lookup"><span data-stu-id="58b71-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="58b71-111">פתיחת הפריט</span><span class="sxs-lookup"><span data-stu-id="58b71-111">Open the item</span></span>
- <span data-ttu-id="58b71-112">קובץ -> מאפיינים -> כותרות אינטרנט</span><span class="sxs-lookup"><span data-stu-id="58b71-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="58b71-113">או</span><span class="sxs-lookup"><span data-stu-id="58b71-113">or</span></span>

<span data-ttu-id="58b71-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="58b71-114">**MFCMapi**</span></span>

- <span data-ttu-id="58b71-115">ניווט אל הפריט בתיבת הדואר הנכנס</span><span class="sxs-lookup"><span data-stu-id="58b71-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="58b71-116">חפש את PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="58b71-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="58b71-117">מאפיינים אלה נקבעים ונרשמו במהלך תעבורה וניתוב.</span><span class="sxs-lookup"><span data-stu-id="58b71-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="58b71-118">לקבלת פתרון בעיות נוסף, ייתכן שיהיה עליך להמשך טיפול בתמיכת תעבורה לגבי הכשלים ב- SPF , DKIM ו- .או DMARC.</span><span class="sxs-lookup"><span data-stu-id="58b71-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>