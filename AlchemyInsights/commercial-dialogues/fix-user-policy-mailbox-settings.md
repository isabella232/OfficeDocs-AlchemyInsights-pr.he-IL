---
title: תיקון הגדרות מדיניות משתמש/תיבת דואר
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034719"
---
# <a name="fix-user-policymailbox-settings"></a>תיקון הגדרות מדיניות משתמש/תיבת דואר

הגדרות דואר הזבל בתיבת הדואר השפיעו על הודעה זו. כדי לסקור את ההגדרות, עשה את הפעולות הבאות:

1. הפעל Exchange ניהול מעטפת. לקבלת מידע נוסף, ראה [פתיחת Exchange ניהול.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. הפעל פקודה זו (באמצעות כתובת הדואר האלקטרוני של המשתמש):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. בדוק אם כתובת הדואר האלקטרוני של השולח היא חלק **מ- TrustedSendersAndDomains** או **BlockedSendersAndDomains**. אם כתובת הדואר האלקטרוני נמצאת באחת מהרשימות, ייתכן שיהיה עליך להסיר אותה. כדי ללמוד עוד, ראה [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
