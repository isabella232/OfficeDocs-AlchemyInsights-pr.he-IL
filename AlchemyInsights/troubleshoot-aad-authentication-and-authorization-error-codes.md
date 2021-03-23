---
title: פתרון בעיות בקודי שגיאה של אימות מודעות מיידיות ואישורים (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036506"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="dbf41-102">פתרון בעיות בקודי שגיאה של אימות מודעות מיידיות ואישורים (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="dbf41-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="dbf41-103">כדי לפתור את האימות או קודי שגיאת ההרשאות של AADSTS, בצע את השלבים המומלצים הבאים:</span><span class="sxs-lookup"><span data-stu-id="dbf41-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="dbf41-104">**טיפול בקודי שגיאה ביישום**</span><span class="sxs-lookup"><span data-stu-id="dbf41-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="dbf41-105">**Oauth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 מספק הנחיות לטיפול בשגיאות במהלך אימות באמצעות חלק השגיאה של תגובת השגיאה.</span><span class="sxs-lookup"><span data-stu-id="dbf41-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="dbf41-106">**שגיאה**: מחרוזת קוד שגיאה שניתן להשתמש בה כדי לסווג סוגים של שגיאות שמתרחשות, ויש להשתמש בהם כדי להגיב לשגיאות.</span><span class="sxs-lookup"><span data-stu-id="dbf41-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="dbf41-107">שדה **השגיאה** מכיל כמה ערכים אפשריים-סקור את קישורי תיעוד הפרוטוקול ומפרט OAuth 2.0 לקבלת מידע נוסף אודות שגיאות ספציפיות וכיצד להגיב להן.</span><span class="sxs-lookup"><span data-stu-id="dbf41-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="dbf41-108">להלן תגובת שגיאה לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="dbf41-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="dbf41-109">**מידע אודות קוד השגיאה הנוכחי של בדיקת מידע**</span><span class="sxs-lookup"><span data-stu-id="dbf41-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="dbf41-110">קודי שגיאה והודעות כפופים לשינוי.</span><span class="sxs-lookup"><span data-stu-id="dbf41-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="dbf41-111">לקבלת המידע העדכני ביותר, עיין https://login.microsoftonline.com/error בעמוד כדי למצוא את תיאורי השגיאות, התיקונים והפתרונות המוצעים של AADSTS.</span><span class="sxs-lookup"><span data-stu-id="dbf41-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="dbf41-112">באפשרותך גם לחפש [קודי שגיאה של AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) ולפתור בעיות המפורטים במאמר [תכלת לספירה וקודי שגיאה של מתן הרשאות](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="dbf41-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="dbf41-113">**קבלת עזרה**</span><span class="sxs-lookup"><span data-stu-id="dbf41-113">**Get Help**</span></span>

- <span data-ttu-id="dbf41-114">[אפשרויות תמיכה ועזרה עבור מפתחים](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -אם אתה זקוק לתשובה לשאלה או לעזרה בפתרון בעיה שאינה מכוסה בתיעוד שלנו, ייתכן שהגיע הזמן להושיט יד למומחים לקבלת עזרה.</span><span class="sxs-lookup"><span data-stu-id="dbf41-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="dbf41-115">מאמר זה מספק כמה הצעות לקבלת תשובות לשאלות שלך בעת פיתוח יישומים המשולבים עם פלטפורמת הזהות של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dbf41-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








