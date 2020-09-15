---
title: כיצד להפוך קבוצות חיצוניות ללא זמינות
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704129"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="eba0d-102">כיצד להפוך קבוצות חיצוניות ללא זמינות</span><span class="sxs-lookup"><span data-stu-id="eba0d-102">How to disable External Groups</span></span>

<span data-ttu-id="eba0d-103">העברת הודעות חיצונית קטרת מחילה כללי תעבורה של Exchange (Etr), ערכה של פקדים מופעלים כדי למנוע מידע אודות החברה להיות משותף.</span><span class="sxs-lookup"><span data-stu-id="eba0d-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="eba0d-104">כדי להגביל את המשתמשים ליצור קבוצות חיצוניות, עליך לקבוע את התצורה של כלל תעבורה של Exchange (ETR) ולאחר מכן לקבוע את התצורה של קטרת כדי להשתמש בכלל תעבורה של Exchange כדי לחסום העברת הודעות חיצונית.</span><span class="sxs-lookup"><span data-stu-id="eba0d-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="eba0d-105">לאחר שיצרת כלל במרכז הניהול של Exchange Online, בצע שלבים אלה כדי להגדיר את ETR להחלה ב-קטרת:</span><span class="sxs-lookup"><span data-stu-id="eba0d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="eba0d-106">היכנס ל-קטרת כמנהל מערכת מאומת, **ובמרכז הניהול של קטרת**, עבור אל ' **תוכן \> והגדרות אבטחה של אבטחה '.**</span><span class="sxs-lookup"><span data-stu-id="eba0d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="eba0d-107">תחת **העברת הודעות חיצוניות**, בחר **אכוף את כללי התעבורה של exchange Online exchange (etr) ב-קטרת.**</span><span class="sxs-lookup"><span data-stu-id="eba0d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="eba0d-108">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="eba0d-108">Choose **Save**.</span></span>

<span data-ttu-id="eba0d-109">לקבלת מידע נוסף, ראה [הפיכת הודעות חיצוניות ללא זמינות ברשת קטרת](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="eba0d-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  