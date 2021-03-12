---
title: הקלטת שיחה של 1:1
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
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733850"
---
# <a name="11-call-recording"></a><span data-ttu-id="05ccd-102">הקלטת שיחה של 1:1</span><span class="sxs-lookup"><span data-stu-id="05ccd-102">1:1 call recording</span></span>

<span data-ttu-id="05ccd-103">מנהלי מערכת צריכים לפעול כעת כדי להמשיך לאפשר למשתמשים להקליט שיחות 1:1.</span><span class="sxs-lookup"><span data-stu-id="05ccd-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="05ccd-104">החל מ-12 באפריל 2021, אנו נתחיל לאכוף את האפשרות החדשה של מדיניות השיחות של Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="05ccd-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="05ccd-105">האפשרות ' הקלטת שיחה ' ב-1:1 כרגע נשלטת על-ידי האפשרות *AllowCloudRecording* במדיניות הפגישה של teams.</span><span class="sxs-lookup"><span data-stu-id="05ccd-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="05ccd-106">אם המשתמשים שלך מורשים לתעד פגישות של Teams, הם יכולים גם לתעד שיחות 1:1.</span><span class="sxs-lookup"><span data-stu-id="05ccd-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="05ccd-107">אם אתה מעדיף לחסום את כל המשתמשים מפני הקלטה של שיחות 1:1, אין צורך לבצע פעולה כלשהי.</span><span class="sxs-lookup"><span data-stu-id="05ccd-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="05ccd-108">האפשרות ' מדיניות שיחות *AllowCloudRecordingForCalls* ' תכלול $False כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="05ccd-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="05ccd-109">שינוי זה מתועד בפרסום מרכז ההודעות הבא: [(מעודכן) 1:1 שיחה מבוא למדיניות הקלטה](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) כדי להגדיר את האפשרות מדיניות שיחות של teams עליך להשתמש ב- [team PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="05ccd-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="05ccd-110">**כדי להפוך הקלטת שיחה לזמינה בשיחות 1:1: Set-CsTeamsCallingPolicy** -Global AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="05ccd-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="05ccd-111">**כדי להפוך הקלטת שיחות ללא זמינה בשיחות 1:1: Set-CsTeamsCallingPolicy** -$False AllowCloudRecordingForCalls</span><span class="sxs-lookup"><span data-stu-id="05ccd-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

