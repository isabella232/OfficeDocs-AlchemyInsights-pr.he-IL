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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314385"
---
# <a name="11-call-recording"></a>הקלטת שיחה ב- 1:1

אם **לחצן התחל הקלטה** מופיע באפור ב- 1:1 שיחה, עליך לשנות את הגדרות המדיניות עבור המשתמש המשפיע. כדי לבדוק את הגדרת המדיניות, הפעל את האבחון עבור המשתמש מושפע על-ידי **הקלדת Diag: Teams 1:1 הקלטת שיחה** לעיל.     

החל מ- 31 במאי 2021, נתחיל לאלץ מדיניות Teams חדשה *AllowCloudRecordingForCalls*. לפני שינוי זה, הקלטת שיחה של 1:1 נשלטת על-ידי מדיניות הפגישות *AllowCloudRecording* Teams פגישה. שינוי זה מתועד בפרסום מרכז ההודעות: [(עדכון) 1:1 מבוא](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)מדיניות הקלטת שיחות .  

*AllowCloudRecordingForCalls*   אפשרות מדיניות שיחות מוגדרת $False **כברירת** מחדל. אם אתה מעדיף לחסום את כל המשתמשים מהקלטה של שיחות 1:1, אין צורך לבצע פעולה כלשהי.  

כדי לאפשר הקלטת שיחות עבור כל המשתמשים ב- 1:1 שיחות, [השתמש Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) כדי להפעיל את ה- cmdlet הבא: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

לחלופין, באפשרותך ליצור מדיניות חדשה ולהגדיר **-AllowCloudRecordingForCalls** **$true ולהקצות** מדיניות זו למשתמשים שלך. 

לקבלת מידע נוסף, ראה [1:1 פקדי מדיניות הקלטת שיחות הם (כמעט!) כאן .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
