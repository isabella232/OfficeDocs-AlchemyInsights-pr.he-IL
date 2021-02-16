---
title: סינכרון קבוצה
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256796"
---
# <a name="group-sync"></a>סינכרון קבוצה

מאמר זה מספק הנחיות לסינכרון קבוצתי.

1. אם אין באפשרותו של מנהל מערכת כללי או של בעלים של קבוצה לשנות מאפייני קבוצה או להוסיף חברים או להקצות בעלים בפורטל התכלת, ודא שמקור הסמכות עבור הקבוצה הוא תכלת Active Directory (תכלת לספירה) עבור בעלי הניהול הכללי או הקבוצה כדי לשנות את הקבוצה.
2. לפני שתנסה למחוק קבוצה מסונכרנת ב-תכלת AD, ודא [שמחקת את כל הרשיונות שהוקצו](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) כדי למנוע שגיאות.

להבנת האופן שבו ניתן לסנכרן משתמשים, קבוצות ואנשי קשר, ראה [הסינכרון של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)ועקוב אחר [סינכרון קבוצה מקומית לתכלת באמצעות תכלת ad connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to סינכרון קבוצות של סלסול באמצעות ad Connect.

בצע את הפעולות הבאות לפתרון בעיות בנושא מדריך זה [במהלך הסינכרון](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) כדי לפתור שגיאות נפוצות

