---
title: פתרון בעיות בדואר אלקטרוני
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569141"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="9a4fd-102">פתרון בעיות בדואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="9a4fd-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="9a4fd-103">ודא שהתכונה מאופשרת עבור תיבת הדואר: מערכת <mailbox></span><span class="sxs-lookup"><span data-stu-id="9a4fd-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="9a4fd-104">לאחר מכן, הביטו ביומני הרישום של ' אירועי דואר אלקטרוני ' <mailbox></span><span class="sxs-lookup"><span data-stu-id="9a4fd-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="9a4fd-105">ביומני ' אירועים מתוך דואר אלקטרוני ', מצא את מזהה ה-Internetהודעה התואם לפריט בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="9a4fd-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="9a4fd-106">תוצאת האמון קובעת אם הפריט נוסף או לא.</span><span class="sxs-lookup"><span data-stu-id="9a4fd-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="9a4fd-107">אירועים יתווספו רק אם האמון בציון = "מהימן".</span><span class="sxs-lookup"><span data-stu-id="9a4fd-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="9a4fd-108">תוצאת האמון נקבעת על-ידי המאפיינים SPF, Dkim או Dkim, הנמצאים בכותרת ההודעה.</span><span class="sxs-lookup"><span data-stu-id="9a4fd-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="9a4fd-109">כדי להציג מאפיינים אלה:</span><span class="sxs-lookup"><span data-stu-id="9a4fd-109">To view these properties:</span></span>

<span data-ttu-id="9a4fd-110">**שולחן העבודה Outlook**</span><span class="sxs-lookup"><span data-stu-id="9a4fd-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="9a4fd-111">פתח את הפריט</span><span class="sxs-lookup"><span data-stu-id="9a4fd-111">Open the item</span></span>
- <span data-ttu-id="9a4fd-112">קובץ-_ Gt_ מאפיינים-_ Gt_ כותרות אינטרנט</span><span class="sxs-lookup"><span data-stu-id="9a4fd-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="9a4fd-113">או</span><span class="sxs-lookup"><span data-stu-id="9a4fd-113">or</span></span>

<span data-ttu-id="9a4fd-114">**מעגל שפיר**</span><span class="sxs-lookup"><span data-stu-id="9a4fd-114">**MFCMapi**</span></span>

- <span data-ttu-id="9a4fd-115">ניווט לפריט בתיבת הדואר הנכנס</span><span class="sxs-lookup"><span data-stu-id="9a4fd-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="9a4fd-116">חפש PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="9a4fd-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="9a4fd-117">מאפיינים אלה נקבעים ונרשמים במהלך הובלה וניתוב.</span><span class="sxs-lookup"><span data-stu-id="9a4fd-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="9a4fd-118">לפתרון בעיות נוסף, ייתכן שיהיה עליך להמשיך בטיפול בתמיכת תעבורה אודות הכשלים ב-SPF, DKIM ו-. או DKIM.</span><span class="sxs-lookup"><span data-stu-id="9a4fd-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>