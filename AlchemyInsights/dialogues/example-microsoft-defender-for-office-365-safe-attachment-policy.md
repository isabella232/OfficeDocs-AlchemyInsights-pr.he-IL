---
title: דוגמה של Microsoft Defender עבור מדיניות הקבצים המצורפים הבטוחה של Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693826"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="c45db-102">דוגמה של Microsoft Defender עבור מדיניות הקבצים המצורפים הבטוחה של Office 365</span><span class="sxs-lookup"><span data-stu-id="c45db-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="c45db-103">הגדרות אלה מאפשרות מדיניות שנקראת *ללא עיכובים* שמעבירה הודעות באופן מיידי ולאחר מכן מצמידות קבצים מצורפים לאחר סריקתן:</span><span class="sxs-lookup"><span data-stu-id="c45db-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="c45db-104">**Name**: ללא עיכובים</span><span class="sxs-lookup"><span data-stu-id="c45db-104">**Name**: No delays</span></span>
- <span data-ttu-id="c45db-105">**תיאור**: מספק הודעות באופן מיידי ומחבר קבצים מצורפים לאחר הסריקה.</span><span class="sxs-lookup"><span data-stu-id="c45db-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="c45db-106">**תגובה**: בחר את אפשרות **המסירה הדינאמית** .</span><span class="sxs-lookup"><span data-stu-id="c45db-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="c45db-107">לקבלת מידע נוסף, ראה [מסירה דינאמית במדיניות קבצים מצורפים בטוחים](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="c45db-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="c45db-108">המקטע **ניתוב מחדש של קובץ מצורף** : בחר את האפשרות **להפיכת ניתוב מחדש לזמין** ולאחר מכן הזן את כתובת הדואר האלקטרוני של מנהל המערכת הכללי של Microsoft 365, מנהל האבטחה או אנליסט האבטחה שיחקרו קבצים מצורפים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="c45db-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="c45db-109">**הוחל** על מקטע: בחר **את תחום הנמען** ולאחר מכן בחר את התחום שלך.</span><span class="sxs-lookup"><span data-stu-id="c45db-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="c45db-110">בחר **הוסף** ולאחר מכן בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="c45db-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="c45db-111">לאחר שתסיים, בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="c45db-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="c45db-112">לקבלת מידע נוסף, ראה [קבצים מצורפים בטוחים ב-Microsoft Defender עבור Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="c45db-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
