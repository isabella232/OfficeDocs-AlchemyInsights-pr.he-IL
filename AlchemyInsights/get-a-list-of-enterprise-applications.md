---
title: קבל רשימה של יישומים ארגוניים
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404931"
---
# <a name="get-a-list-of-enterprise-applications"></a>קבל רשימה של יישומים ארגוניים

1. כדי **לקבל רשימה של יישומים ארגוניים** (כל היישומים או מסוננים לפי שם תצוגה, מזהה, מזהי כתובות URL וכדומה) באמצעות הפקודה Powershell, ראה [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. כדי לקבל רשימה של אובייקטים ראשיים של שירות (כל האובייקטים או המסוננים לפי מזהה) באמצעות הפקודה Powershell, ראה [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. אם ברצונך לקבל רשימה **של אפליקציות המוגדרות על-ידי SAML, ייתכן שקבצי Script של PowerShell הבאים** יעזרו לך:

    כל יישום הוא יישום OAuth או יישום SAML (הן גלריה וגם אפליקציות שאינן גלריה) כוללים שני אובייקטים שנוצרו ב- AAD כאשר הרישום שלהם מתרחש. אובייקט אחד נקרא אובייקט היישום והאובייקט השני הוא האובייקט הראשי של השירות. בעת השלכת המאפיינים של אובייקט ראשי של שירות באמצעות PowerShell, תגלה שלכל יישום יש מספר מסוים של תגיות המשויכות לו, כמו:

    - יישומי OAuth כוללים תגית בשם "**WindowsAzureActiveDirectoryIntegratedApp**"
    - אפליקציות SAML של גלריה כוללות תגית בשם "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - אפליקציות SAML שאינן גלריה כוללות תגית בשם "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    לפיכך, באפשרותך להשתמש בתגיות אלה ולברר איזה סוג יישום זה. התגית "**WindowsAzureActiveDirectoryIntegratedApp**" נפוצה בכל סוגי האפליקציות. באפשרותך להשתמש במקטעי הבאים כדי רשימת כל יישומי SAML (הן גלריה וגם לא גלריה):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    לקבלת מידע נוסף, ראה [זיהוי יישומים התומכים ב- SAML ב- Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **חיפוש ורשימה של יישומי אינטרנט בלבד:** השתמש בפקודה שלהלן כדי לקבל את כל יישומי Azure AD עם סוג היישום "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **חפש והצג רשימה של יישומים מקוריים** בלבד: הפעל את הפקודה הבאה כדי לקבל את כל יישומי הלקוח המקורי (מחשב שולחני/מכשיר נייד).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **ייצא את כל פרטי היישום של Azure AD הרשומים ל- CSV**: הפקודה שלהלן מייצאת את כל יישומי Azure AD עם הפרטים הדרושים לקובץ csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **צריך לייצא רשימה של יישומים של Azure שלא נוסו** – ביקורת הדוח

    Azure AD יכול להציג יומני יישומים עבור עד 30 יום בלבד בתנאי שיש לך רשיון Azure AD Premium.
    יש לך שתי אפשרויות לשמור את הנתונים במשך יותר מ- 30 יום. באפשרותך להשתמש ב- [API של דיווח Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) כדי לאחזר את הנתונים באופן תיכנותי ולאחסן אותם במסד נתונים. לחלופין, באפשרותך לשלב יומני ביקורת במערכת סיאם של ספקים שלישיים.

    באפשרותך גם להוריד את רשימת היישומים עבור כל היישומים והיישומים שבבעלותם תחת Azure Active directory>רישום יישומים>הורד>כל היישומים/יישומים בבעלות.

    כדי לקבל רשימה של יישומים באמצעות MS Graph, ראה רשימת יישומים [- Microsoft Graph v1.0 וסוג](https://docs.microsoft.com/graph/api/application-list) משאב יישום - Microsoft [Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
