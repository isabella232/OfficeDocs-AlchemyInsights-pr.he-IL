---
title: כיצד להשבית קבוצות חיצוני
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384826"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="c70f6-102">כיצד להשבית קבוצות חיצוני</span><span class="sxs-lookup"><span data-stu-id="c70f6-102">How to disable External Groups</span></span>

<span data-ttu-id="c70f6-103">Yammer העברת הודעות החיצוני מחיל כללי התעבורה Exchange (ETRs), קבוצה של פקדי מקדימים כדי למנוע מידע חברה משותפת.</span><span class="sxs-lookup"><span data-stu-id="c70f6-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="c70f6-104">כדי להגביל את המשתמשים מיצירת קבוצות חיצוני, עליך לקבוע את התצורה של כלל התעבורה Exchange (ETR) ולאחר מכן הגדר Yammer לשימוש כלל התעבורה Exchange כדי לחסום הודעות חיצוני.</span><span class="sxs-lookup"><span data-stu-id="c70f6-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="c70f6-105">לאחר שיצרת כלל במרכז הניהול של Exchange Online, בצע את השלבים הבאים כדי להגדיר ETR להחלת ב- Yammer:</span><span class="sxs-lookup"><span data-stu-id="c70f6-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="c70f6-106">כניסה ל- Yammer כמנהל מאומת, וב - **Yammer מרכז admin**, עבור אל C **תוכן ואבטחה \> הגדרות האבטחה.**</span><span class="sxs-lookup"><span data-stu-id="c70f6-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="c70f6-107">תחת **הודעות חיצוניים**, בחר **לאכוף Exchange Online Exchange תעבורה הכללים שלך (ETRs) ב- Yammer.**</span><span class="sxs-lookup"><span data-stu-id="c70f6-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="c70f6-108">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="c70f6-108">Choose **Save**.</span></span>

<span data-ttu-id="c70f6-109">לקבלת מידע נוסף, ראה [שליטה חיצוני בהודעות רשת Yammer עם כללי התעבורה Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="c70f6-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  