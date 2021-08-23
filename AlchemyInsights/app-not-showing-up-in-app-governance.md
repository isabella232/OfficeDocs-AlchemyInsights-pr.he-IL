---
title: האפליקציה שלי אינה מופיעה ב'ממשל אפליקציה'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454698"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>האפליקציה שלי אינה מופיעה ב'ממשל אפליקציה'

אם היישום שלך אינו מופיע ב- App Governance, בדוק את הפעולות הבאות:

1. עבור אל [Azure AD](https://aad.portal.azure.com/) ומצא את מזהה היישום עבור היישום שלך על-ידי חיפוש שם היישום העליונה בדף מבט כולל.

1. Access Graph Explorer וחפש את מזהה היישום בתוך מנהל השירות שלך באמצעות שאילתה זו והחלפה במזהה היישום <appId> הרלוונטי: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. אם לא מוחזרות תוצאות, חפש את מזהה היישום בתוך היישום באמצעות שאילתה זו והחלפה במזהה היישום <appId> הרלוונטי: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

אם אתה נתקל בבעיות בשאילתה, ראה [קבל תמיכה](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

לקבלת מידע נוסף או תובנות לגבי האפליקציות שלך ב'ממשל יישומים', [ראה מידע על ניראות ותובנות](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview).

לקבלת מידע נוסף אודות הצגת האפליקציות שלך, ראה [הצגת האפליקציות שלך.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
