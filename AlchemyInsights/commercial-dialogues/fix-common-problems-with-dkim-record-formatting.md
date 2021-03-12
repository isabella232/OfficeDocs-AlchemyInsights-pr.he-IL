---
title: פתרון בעיות נפוצות בעיצוב רשומות של DKIM
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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746835"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>פתרון בעיות נפוצות בעיצוב רשומות של DKIM

רוב בעיות ההגדרה של DKIM קשורות לרשומות DNS שגויות.

כדי לפתור את בעיות ההגדרה של DKIM, ודא שרשומת CNAME של DKIM (**לא** רשומת TXT) מעוצבת כראוי. לקבלת מידע נוסף, ראה [מה עליך לעשות כדי להגדיר את DKIM באופן ידני ב-Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

אם אתה זקוק לעזרה בנוגע לרשומות DNS באופן כללי, ראה [יצירת רשומות dns בכל ספק אירוח dns עבור Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> לאחר שתיצור או תעדכן את רשומות ה-DNS שלך ב-DKIM בשירות אירוח ה-DNS עבור התחום שלך, יהיה עליך להמתין עד להפיץ את רשומות ה-DNS.
