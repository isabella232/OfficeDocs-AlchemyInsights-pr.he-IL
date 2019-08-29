---
title: S/MIME ב- Outlook באינטרנט
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666841"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="90575-102">הצפנת הודעות דואר אלקטרוני ב- Outlook</span><span class="sxs-lookup"><span data-stu-id="90575-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="90575-103">הצפנת הודעת office 365 בנוי על Microsoft תכלת הרקיע ניהול זכויות (RMS תכלת הרקיע), המהווה חלק תכלת הרקיע הגנת מידע.</span><span class="sxs-lookup"><span data-stu-id="90575-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="90575-104">אם המנוי שלך כולל ניהול זכויות תכלת הרקיע או הגנה על המידע תכלת הרקיע, **אינך צריך לבצע את כל הפעולות כדי להפעיל באופן ידני או להפעיל** שירות ניהול זכויות.</span><span class="sxs-lookup"><span data-stu-id="90575-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="90575-105">בהתבסס על משוב הלקוחות, אנו עוד אפשרות הפעלת כללי זרימת דואר של Exchange להצפין באופן אוטומטי דואר אלקטרוני יוצאת המכילה סוג מסוים של מידע רגיש בדיירים שלך כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="90575-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="90575-106">במקום זאת, אנו מספקים הוראות מפורטות אודות האופן שבו ניתן לעשות זאת לעצמך.</span><span class="sxs-lookup"><span data-stu-id="90575-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="90575-107">לקבלת פרטים נוספים אודות אופן היצירה של כלל התעבורה להצפנת מידע רגיש, עיין [במאמר זה](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="90575-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="90575-108">אם משתמש ב- Outlook באינטרנט (לשעבר **OWA**): בעת חיבור הודעת דואר אלקטרוני, פשוט לחץ על **הגנה** ב- OWA.</span><span class="sxs-lookup"><span data-stu-id="90575-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="90575-109">פעולה זו תחיל את ההרשאה "אל תעביר לנמענים".</span><span class="sxs-lookup"><span data-stu-id="90575-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="90575-110">לחץ על **שינוי הרשאה** ובחרו ' **הצפן** להצפנת ההודעה בלבד.</span><span class="sxs-lookup"><span data-stu-id="90575-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="90575-111">אם משתמש **בלקוח Outlook**: כדי לשלוח הודעה מוצפנת מ- Outlook 2013 או 2016, או Outlook 2016 עבור Mac, בחר **באפשרויות** > **הרשאות**ולאחר מכן בחר את האפשרות הגנה עליך.</span><span class="sxs-lookup"><span data-stu-id="90575-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="90575-112">כדי **להצפין באופן אוטומטי כל דואר אלקטרוני** שנשלחו לנמענים או ארגונים שותפים חיצוניים מסוימים, עליך ליצור כלל תעבורה זרימת דואר במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="90575-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="90575-113">הוראות מפורטות מובאות במאמר [תמיכה זה](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="90575-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

