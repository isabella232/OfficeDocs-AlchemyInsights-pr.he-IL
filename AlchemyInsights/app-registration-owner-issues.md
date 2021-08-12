---
title: בעיות של בעלים של רישום אפליקציה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951134"
---
# <a name="app-registration-owner-issues"></a>בעיות של בעלים של רישום אפליקציה

להלן השיטות הזמינות להוספת מנהלים כבעלים עבור רישומי אפליקציות:

- שימוש במודול Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    הפניה: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- שימוש ב- Azure CLI - `az ad app owner add`

    הפניה: [הבעלים של אפליקציית המודעות az](https://docs.microsoft.com/cli/azure/ad/app/owner)
- שימוש ב- MS Graph -

    הפניה: [הוספת בעלים - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- שימוש בפורטל Azure AD - נווט [אל portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > בחר את היישום שלך > בעלים > הוסף בעלים

**לא ניתן להציג את היישום שלך בלהב 'רישומי אפליקציה' למרות שאתה הבעלים של יישום זה?**

הבעלים של יישום אינו תפקיד ניהולי. אם ההגדרה [הגבל גישה לפורטל](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) הניהול של Azure AD זמינה, רק מנהל המערכת יוכל להציג את היישומים בפורטל רישום יישומים. כדי שהבעלים יוכל להציג את היישומים, הפוך הגדרה זו ללא זמינה (הגדר הגדרה זו ללא) או הקצה תפקיד מנהל מערכת לבעלים עבור היישום הספציפי בלבד. עם זאת, תדרוש רשיון Azure AD Premium P2 ותאפשר [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
