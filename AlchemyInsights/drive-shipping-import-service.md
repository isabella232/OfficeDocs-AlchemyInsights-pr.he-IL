---
title: נהיגה במשלוח בשירות Microsoft 365 ייבוא
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731649"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="6879a-102">נהיגה במשלוח בשירות Microsoft 365 ייבוא</span><span class="sxs-lookup"><span data-stu-id="6879a-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="6879a-103">השתמש במשלוח כונן על-ידי העתקת PSTs לכונן קשיח ולאחר מכן משלוח הכונן הקשיח ל- Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6879a-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="6879a-104">כדי להתחיל את המשימה:</span><span class="sxs-lookup"><span data-stu-id="6879a-104">To start the job:</span></span>

1. <span data-ttu-id="6879a-105">במרכז Microsoft 365 תחת ניהול **מידע**, בחר **ייבוא**.</span><span class="sxs-lookup"><span data-stu-id="6879a-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="6879a-106">בחר **בחר סוג משימה של ייבוא** ולאחר מכן בחר **הבא**.</span><span class="sxs-lookup"><span data-stu-id="6879a-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="6879a-107">כדי לראות את השלבים עבור אפשרות ייבוא זו, בחר **שלח כוננים קשיחים לאחד מהמיקום הפיזי שלנו**.</span><span class="sxs-lookup"><span data-stu-id="6879a-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="6879a-108">להלן כמה דברים שיש לזכור:</span><span class="sxs-lookup"><span data-stu-id="6879a-108">Here are some things to remember:</span></span>

- <span data-ttu-id="6879a-109">יש להקצות את התפקיד 'ייצוא ייבוא תיבת דואר' ב- Exchange Online כדי לייבא קבצי PST לתיבות Microsoft 365 הדואר.</span><span class="sxs-lookup"><span data-stu-id="6879a-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="6879a-110">ייתכן שהביצועים מושפעים עבור PSTs שגודלם עולה על 20 ג'יגה-בתים.</span><span class="sxs-lookup"><span data-stu-id="6879a-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="6879a-111">נתמכים רק כונני Solid-state (SSD) בגודל 2.5 אינץ' או כוננים קשיחים פנימיים מסוג SATA II/III בגודל 2.5 אינץ' או 3.5 אינץ'.</span><span class="sxs-lookup"><span data-stu-id="6879a-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="6879a-112">יש להצפין את הכונן הקשיח המכיל קבצי PST באמצעות BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6879a-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="6879a-113">העלות לייבוא קבצי PST לתיבות Microsoft 365 באמצעות משלוח כונן היא $2 דולר ארה"ב לכל GB של נתונים.</span><span class="sxs-lookup"><span data-stu-id="6879a-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="6879a-114">לקבלת מידע נוסף אודות השימוש בשיטת המשלוח של Drive לייבוא קבצי PSTs, ראה [שימוש במשלוח כונן כדי לייבא](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)קבצי PST של הארגון שלך .</span><span class="sxs-lookup"><span data-stu-id="6879a-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>