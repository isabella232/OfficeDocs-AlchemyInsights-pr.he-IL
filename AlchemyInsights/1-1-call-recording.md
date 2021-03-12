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
# <a name="11-call-recording"></a>הקלטת שיחה של 1:1

מנהלי מערכת צריכים לפעול כעת כדי להמשיך לאפשר למשתמשים להקליט שיחות 1:1.
 
החל מ-12 באפריל 2021, אנו נתחיל לאכוף את האפשרות החדשה של מדיניות השיחות של Teams *AllowCloudRecordingForCalls*. 

האפשרות ' הקלטת שיחה ' ב-1:1 כרגע נשלטת על-ידי האפשרות *AllowCloudRecording* במדיניות הפגישה של teams. אם המשתמשים שלך מורשים לתעד פגישות של Teams, הם יכולים גם לתעד שיחות 1:1.

אם אתה מעדיף לחסום את כל המשתמשים מפני הקלטה של שיחות 1:1, אין צורך לבצע פעולה כלשהי. האפשרות ' מדיניות שיחות *AllowCloudRecordingForCalls* ' תכלול $False כברירת מחדל.

שינוי זה מתועד בפרסום מרכז ההודעות הבא: [(מעודכן) 1:1 שיחה מבוא למדיניות הקלטה](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) כדי להגדיר את האפשרות מדיניות שיחות של teams עליך להשתמש ב- [team PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**כדי להפוך הקלטת שיחה לזמינה בשיחות 1:1: Set-CsTeamsCallingPolicy** -Global AllowCloudRecordingForCalls $True

**כדי להפוך הקלטת שיחות ללא זמינה בשיחות 1:1: Set-CsTeamsCallingPolicy** -$False AllowCloudRecordingForCalls

