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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540902"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="07cf5-102">כיצד להשבית קבוצות חיצוני</span><span class="sxs-lookup"><span data-stu-id="07cf5-102">How to disable External Groups</span></span>

<span data-ttu-id="07cf5-103">Yammer העברת הודעות החיצוני מחיל כללי התעבורה Exchange (ETRs), קבוצה של פקדי מקדימים כדי למנוע מידע חברה משותפת.</span><span class="sxs-lookup"><span data-stu-id="07cf5-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="07cf5-104">כדי להגביל את המשתמשים מיצירת קבוצות חיצוני, עליך לקבוע את התצורה של כלל התעבורה Exchange (ETR) ולאחר מכן הגדר Yammer לשימוש כלל התעבורה Exchange כדי לחסום הודעות חיצוני.</span><span class="sxs-lookup"><span data-stu-id="07cf5-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="07cf5-105">לאחר שיצרת כלל במרכז הניהול של Exchange Online, בצע את השלבים הבאים כדי להגדיר ETR להחלת ב- Yammer:</span><span class="sxs-lookup"><span data-stu-id="07cf5-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="07cf5-106">כניסה ל- Yammer כמנהל מאומת, וב - **Yammer מרכז admin**, עבור אל C **תוכן ואבטחה \> הגדרות האבטחה.**</span><span class="sxs-lookup"><span data-stu-id="07cf5-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="07cf5-107">תחת **הודעות חיצוניים**, בחר **לאכוף Exchange Online Exchange תעבורה הכללים שלך (ETRs) ב- Yammer.**</span><span class="sxs-lookup"><span data-stu-id="07cf5-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="07cf5-108">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="07cf5-108">Choose **Save**.</span></span>

<span data-ttu-id="07cf5-109">לקבלת מידע נוסף, ראה [שליטה חיצוני בהודעות רשת Yammer עם כללי התעבורה Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="07cf5-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  