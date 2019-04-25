---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383836"
---
# <a name="content-search-not-returning-expected-results"></a>חיפוש תוכן שלא להחזיר את התוצאות הצפויות

בעת הפעלת תוכן חיפושים מ & האבטחה של Office 365 מרכז תאימות, ייתכן שתקבל תוצאות החיפוש לא צפויה. עליך לשקול את הדברים הבאים שיכולים להשפיע על תוצאות החיפוש שלך:

- **מיקומי תוכן ואת תנאי חיפוש**: ודא שבחרת את מיקומי תוכן המתאים ואת תנאי חיפוש. אם הפעלת חיפוש גדולים (עם מיקומים רבים), שתשקול לפצל אותו לתוך חיפושים מרובים.

- **פריטים כלולים באינדקס חלקית**: [פריטים כלולים באינדקס באופן חלקי](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) מתיבות נכללים בתוצאות החיפוש משוער. עם זאת, פריטי אינדקס חלקית מאתרי SharePoint ואת OneDrive שאינם נכללים במרכז ההערכה החיפוש.

- **כשלים החיפוש**: בעת חיפוש מספר גדול של תיבות דואר (מעל ל- 100,000 תיבות דואר), אתה מקבל שגיאות החיפוש, עם קודי שגיאה כגון CS008-009 ו- CS012-002). במקרה זה, נסה שנית את החיפוש רק עבור מיקומי תוכן נכשלה. עיין [במאמר זה](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) לקבלת מידע נוסף.
