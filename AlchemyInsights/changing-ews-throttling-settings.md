---
title: שינוי הגדרות ויסות EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818037"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="4d7be-102">שינוי הגדרות ויסות EWS</span><span class="sxs-lookup"><span data-stu-id="4d7be-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="4d7be-103">הפעל את הבדיקה האוטומטית שלנו שתאפשר לך לשנות את מדיניות הוויסות של EWS למשך זמן ההעברה.</span><span class="sxs-lookup"><span data-stu-id="4d7be-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="4d7be-104">שים לב, גם לאחר הפעלת אפשרות זו, פעולות הייבוא של EWS עדיין יהיו מוגבלות ל- 150mb לכל 5 דקות לכל תיבת דואר; כדי להשיג מהירויות תפוקת העברה גבוהות יותר, העבר יותר משתמשים במקביל.</span><span class="sxs-lookup"><span data-stu-id="4d7be-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="4d7be-105">שים לב ששינויי מדיניות הוויסות של EWS לא משפיעים על סוגי ההעברה הבאים (באמצעות כלי Microsoft): העברה היברידית, בשלב אחד/בשלבים (RPC/HTTP), IMAP,‏ G Suite, תיקיה ציבורית או שירות ייבוא PST.</span><span class="sxs-lookup"><span data-stu-id="4d7be-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>