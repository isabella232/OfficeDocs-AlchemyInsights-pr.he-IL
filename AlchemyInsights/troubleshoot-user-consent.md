---
title: פתרון בעיות בהסכמת משתמש
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007899"
---
# <a name="troubleshoot-user-consent"></a>פתרון בעיות בהסכמת משתמש

1. באפשרותך לקבוע את התצורה של ההסכמה של משתמשי קצה ליישומים באמצעות Azure Portal או PowerShell. לקבלת [מידע נוסף, ראה הגדרות](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) הסכמת משתמש.
1. מנהל מערכת יכול גם להשתמש [ב- API Graph Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) כדי להעניק הסכמה להרשאות שהוקצו בשמו של משתמש יחיד. לקבלת מידע נוסף, [ראה קבל גישה בשם משתמש](https://docs.microsoft.com/graph/auth-v2-user).
1. [שגיאות בהסכמת](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)משתמש : מאמר זה דן בשגיאות שעלולות להתרחש במהלך תהליך ההסכמה ליישום. אם אתה פותר בעיות של בקשות הסכמה בלתי צפויות שלא מכילות הודעות שגיאה, ראה [תרחישי אימות עבור Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).