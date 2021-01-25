---
title: בעיית הקצאת משאבים של SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949787"
---
# <a name="scim-provisioning-issue"></a>בעיית הקצאת משאבים של SCIM

הקצאת משאבים אוטומטית מתייחסת ליצירת זהויות משתמשים ותפקידים ביישומי הענן שהמשתמשים זקוקים להם לגישה אליהם. בנוסף ליצירת זהויות משתמשים, הקצאת משאבים אוטומטית כוללת את התחזוקה וההסרה של זהויות משתמשים כאשר מצב או תפקידים משתנים. לפני שתתחיל בפריסה, באפשרותך לבדוק [כיצד](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) הקצאת המשאבים פועלת כדי ללמוד כיצד פועלת ההקצאה של תכלת active DIRECTORY (AD) וקבלת המלצות תצורה.

כמפתח יישומים, באפשרותך להשתמש במערכת עבור API של ניהול זהויות בין תחומים (SCIM) עבור ניהול משתמשים כדי לאפשר הקצאה אוטומטית של משתמשים וקבוצות בין היישום שלך לבין תכלת לספירה. [נקודת הקצה של BUILD SCIM וקביעת תצורה של הקצאת משאבים באמצעות מאמר תכלת לספירה](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) מתארת כיצד לבנות נקודת קצה של SCIM ולשלב אותה עם שירות הקצאת המשאבים של תכלת לספירה.



