---
title: S/MIME ב-Outlook באינטרנט
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772263"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="13a48-102">הצפנת הודעות דואר אלקטרוני ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="13a48-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="13a48-103">הצפנת ההודעות של microsoft 365 מבוססת על ניהול זכויות של Microsoft תכלת (תכלת RMS), המהווה חלק מהגנה על מידע של תכלת.</span><span class="sxs-lookup"><span data-stu-id="13a48-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="13a48-104">אם המנוי שלך כולל הגנה על זכויות תכלת או הגנה על מידע תכלת, **אין צורך לבצע פעולות כלשהן כדי להפעיל או להפעיל** את שירות ניהול הזכויות באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="13a48-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="13a48-105">בהתבסס על משוב הלקוחות, לא נאפשר עוד כללי זרימת דואר של Exchange כדי להצפין באופן אוטומטי דואר אלקטרוני יוצא המכיל סוג מסוים של מידע רגיש בדייר שלך כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="13a48-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="13a48-106">במקום זאת, אנו מספקים הוראות מפורטות לגבי האופן שבו תוכל לעשות זאת בעצמך.</span><span class="sxs-lookup"><span data-stu-id="13a48-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="13a48-107">לקבלת פרטים נוספים על יצירת כלל תעבורה להצפנת מידע רגיש, עיין [במאמר זה](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="13a48-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="13a48-108">אם אתה משתמש ב-Outlook באינטרנט (לשעבר **OWA**): בעת חיבור הודעת דואר אלקטרוני, פשוט לחץ על **הגן** ב-owa.</span><span class="sxs-lookup"><span data-stu-id="13a48-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="13a48-109">פעולה זו תחול על הרשאת "אל תעביר".</span><span class="sxs-lookup"><span data-stu-id="13a48-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="13a48-110">לחץ על **שינוי הרשאה** ובחר באפשרות **הצפן** כדי להצפין את ההודעה בלבד.</span><span class="sxs-lookup"><span data-stu-id="13a48-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="13a48-111">אם אתה משתמש **ב-outlook client**: כדי לשלוח הודעה מוצפנת מ-outlook 2013 או 2016, או outlook 2016 עבור Mac, בחר **Options**  >  **הרשאות**אפשרויות ולאחר מכן בחר את אפשרות ההגנה הדרושה.</span><span class="sxs-lookup"><span data-stu-id="13a48-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="13a48-112">כדי **להצפין באופן אוטומטי את כל הדואר האלקטרוני** שנשלח לנמענים מסוימים או לארגונים שותפים חיצוניים, עליך ליצור כלל תעבורה של זרימת דואר במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="13a48-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="13a48-113">הוראות מפורטות מוצגות [במאמר תמיכה זה](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="13a48-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

