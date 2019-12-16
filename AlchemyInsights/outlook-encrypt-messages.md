---
title: S/MIME ב-Outlook באינטרנט
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053226"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="044ac-102">הצפן הודעות דואר אלקטרוני ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="044ac-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="044ac-103">הצפנת הודעות של Office 365 מובנית בניהול זכויות תכלת של מיקרוסופט (כחול RMS), המהווה חלק מהגנת המידע התכלת.</span><span class="sxs-lookup"><span data-stu-id="044ac-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="044ac-104">אם המנוי שלך כולל ניהול זכויות תכלת או הגנת מידע תכלת, **אין צורך לבצע פעולות כלשהן כדי להפעיל או להפעיל** את שירות ניהול הזכויות באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="044ac-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="044ac-105">בהתבסס על משוב לקוחות, אנחנו כבר לא מאפשרים Exchange כללי זרימת דואר להצפין באופן אוטומטי דואר אלקטרוני יוצא המכיל סוג מסוים של מידע רגיש בדייר שלך כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="044ac-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="044ac-106">במקום זאת, אנו מספקים הוראות מפורטות לגבי האופן שבו אתם יכולים לעשות זאת בעצמכם.</span><span class="sxs-lookup"><span data-stu-id="044ac-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="044ac-107">לקבלת פרטים נוספים על אופן יצירת כלל תעבורה להצפנת מידע רגיש, עיין [במאמר זה](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="044ac-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="044ac-108">אם אתה משתמש ב-Outlook באינטרנט (לשעבר **OWA**): בעת חיבור הודעת דואר אלקטרוני, פשוט לחץ על **הגן** ב-OWA.</span><span class="sxs-lookup"><span data-stu-id="044ac-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="044ac-109">פעולה זו תגרום להחלת הרשאת "אל תעביר".</span><span class="sxs-lookup"><span data-stu-id="044ac-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="044ac-110">לחץ על **שנה הרשאה** ובחר באפשרות **הצפן** כדי להצפין את ההודעה בלבד.</span><span class="sxs-lookup"><span data-stu-id="044ac-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="044ac-111">אם נעשה שימוש **בלקוח outlook**: כדי לשלוח הודעה מוצפנת מ-outlook 2013 או 2016, או outlook 2016 for Mac, בחר**הרשאות** **אפשרויות** > ולאחר מכן בחר באפשרות ההגנה הדרושה.</span><span class="sxs-lookup"><span data-stu-id="044ac-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="044ac-112">כדי **להצפין באופן אוטומטי את כל הדואר האלקטרוני** שנשלח לנמענים מסוימים או לארגונים חיצוניים שותפים, עליך ליצור כלל הובלה של זרימת דואר במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="044ac-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="044ac-113">הוראות מפורטות מסופקות [במאמר זה תמיכה](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="044ac-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

