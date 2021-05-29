---
title: הקלטת שיחה ב- 1:1
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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702091"
---
# <a name="11-call-recording"></a><span data-ttu-id="d69be-102">הקלטת שיחה ב- 1:1</span><span class="sxs-lookup"><span data-stu-id="d69be-102">1:1 call recording</span></span>

<span data-ttu-id="d69be-103">אם **לחצן התחל הקלטה** מופיע באפור ב- 1:1 שיחה, עליך לשנות את הגדרות המדיניות עבור המשתמש המשפיע.</span><span class="sxs-lookup"><span data-stu-id="d69be-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="d69be-104">כדי לבדוק את הגדרת המדיניות, הפעל את האבחון עבור המשתמש מושפע על-ידי **הקלדת Diag: Teams 1:1 הקלטת שיחה** לעיל.</span><span class="sxs-lookup"><span data-stu-id="d69be-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="d69be-105">החל מ- 31 במאי 2021, נתחיל לאלץ מדיניות שיחות Teams *אפשרCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="d69be-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="d69be-106">לפני שינוי זה, הקלטת שיחה של 1:1 נשלטת על-ידי מדיניות Teams *AllowCloudRecording.*</span><span class="sxs-lookup"><span data-stu-id="d69be-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="d69be-107">שינוי זה מתועד בפרסום מרכז ההודעות: [(עדכון) 1:1 מבוא](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)מדיניות הקלטת שיחות .</span><span class="sxs-lookup"><span data-stu-id="d69be-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="d69be-108">*AllowCloudRecordingForCalls*   אפשרות מדיניות שיחות מוגדרת $False **כברירת** מחדל.</span><span class="sxs-lookup"><span data-stu-id="d69be-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="d69be-109">אם אתה מעדיף לחסום את כל המשתמשים מהקלטה של שיחות 1:1, אין צורך לבצע פעולה כלשהי.</span><span class="sxs-lookup"><span data-stu-id="d69be-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="d69be-110">כדי לאפשר הקלטת שיחות עבור כל המשתמשים ב- 1:1 [שיחות, השתמש Teams PowerShell](/microsoftteams/teams-powershell-install) כדי להפעיל את ה- cmdlet הבא:</span><span class="sxs-lookup"><span data-stu-id="d69be-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="d69be-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="d69be-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="d69be-112">לחלופין, באפשרותך ליצור מדיניות חדשה ולהגדיר **-AllowCloudRecordingForCalls** **$true ולהקצות** מדיניות זו למשתמשים שלך.</span><span class="sxs-lookup"><span data-stu-id="d69be-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="d69be-113">לקבלת מידע נוסף, ראה [1:1 פקדי מדיניות הקלטת שיחות הם (כמעט!) כאן .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="d69be-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
