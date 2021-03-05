---
title: חסימת חתימות דואר אלקטרוני שנוצרו על-ידי המשתמש
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482314"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="24974-102">חסימת חתימות דואר אלקטרוני שנוצרו על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="24974-102">Block user-made email signatures</span></span>

<span data-ttu-id="24974-103">הפתרון הבא חל רק על חתימות דואר אלקטרוני שנוצרו ב-Outlook באינטרנט.</span><span class="sxs-lookup"><span data-stu-id="24974-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="24974-104">באפשרותך לחסום רק חתימות באפליקציית Outlook אם יש לך שרת Exchange מקומי.</span><span class="sxs-lookup"><span data-stu-id="24974-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="24974-105">במרכז הניהול, בחר החלפת **מרכזי ניהול**  >  .</span><span class="sxs-lookup"><span data-stu-id="24974-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="24974-106">לחץ על **הרשאות**  >  **מדיניות Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="24974-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="24974-107">בחר את המדיניות ולאחר מכן לחץ על סמל העיפרון כדי לערוך אותו.</span><span class="sxs-lookup"><span data-stu-id="24974-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="24974-108">לחץ על **תכונות**  >  **נוספות**.</span><span class="sxs-lookup"><span data-stu-id="24974-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="24974-109">תחת **חוויית משתמש**, נקה את תיבת הסימון **חתימת דואר אלקטרוני** ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="24974-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="24974-110">**חשוב:** אם נוספה חתימה לפני ניקוי תיבת סימון זו, המשתמש עדיין יוכל להשתמש בו.</span><span class="sxs-lookup"><span data-stu-id="24974-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="24974-111">בקש ממנו להסיר אותו.</span><span class="sxs-lookup"><span data-stu-id="24974-111">Ask them to remove it.</span></span>
