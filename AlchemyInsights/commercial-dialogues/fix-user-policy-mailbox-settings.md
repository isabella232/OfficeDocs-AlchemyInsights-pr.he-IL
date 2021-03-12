---
title: תיקון הגדרות מדיניות המשתמש/תיבת הדואר
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746728"
---
# <a name="fix-user-policymailbox-settings"></a>תיקון הגדרות מדיניות המשתמש/תיבת הדואר

הגדרות ' דואר זבל ' בתיבת הדואר השפיעו על הודעה זו. כדי לסקור את ההגדרות, בצע את הפעולות הבאות:

1. הפעל את מעטפת ניהול Exchange. לקבלת מידע נוסף, ראה [פתיחת מעטפת ניהול Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
2. הפעיל פקודה זו (באמצעות כתובת הדואר האלקטרוני של המשתמש):  **get-mailboxjunkmailconfiguration-identity "user@domain.com"**
3. בדוק אם כתובת הדואר האלקטרוני של השולח היא חלק מ- **TrustedSendersAndDomains** או מ- **BlockedSendersAndDomains**. אם כתובת הדואר האלקטרוני נמצאת באחת מהרשימות, ייתכן שתצטרך להסיר אותה. לקבלת מידע נוסף, ראה [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
