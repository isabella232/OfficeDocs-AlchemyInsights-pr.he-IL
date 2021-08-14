---
title: פתרון בעיות נפוצות בעיצוב רשומות DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930062"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>פתרון בעיות נפוצות בעיצוב רשומות DKIM

רוב בעיות הגדרת DKIM קשורות ברשומות DNS שגויות.

כדי לפתור את בעיות הגדרת DKIM, ודא כי רשומת DKIM CNAME (**לא** רשומת TXT) מעוצבת כראוי. לקבלת מידע נוסף, ראה מה עליך לעשות כדי להגדיר [באופן ידני את DKIM ב- Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

אם אתה זקוק לעזרה עבור רשומות DNS באופן כללי, [ראה יצירת רשומות DNS בכל ספק אירוח DNS עבור Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> לאחר יצירה או עדכון של רשומות ה- DNS של DKIM בשירות אירוח ה- DNS עבור התחום שלך, יהיה עליך להמתין עד להפצת רשומות ה- DNS.
