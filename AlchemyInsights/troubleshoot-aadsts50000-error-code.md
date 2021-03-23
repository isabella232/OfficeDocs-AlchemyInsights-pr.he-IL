---
title: פתרון בעיות בקוד השגיאה של AADSTS50000
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
- "9801"
- "9005744"
ms.openlocfilehash: 63689ea5afea7c6921c93f2ead2350f87c2defa8
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036503"
---
# <a name="troubleshoot-aadsts50000-error-code"></a>פתרון בעיות בקוד השגיאה של AADSTS50000

כדי לפתור את השגיאה AADSTS50000, בצע את השלב הבא:

**AADSTS50000**: TokenIssuanceError-קיימת בעיה עם שירות הכניסה.

אם בקשת האסימון של access חוקית ומורשית, שרת ההרשאות מנפיק אסימון גישה ואסימון רענון אופציונלי. אם הבקשה של אימות לקוח נכשלה או שאינה חוקית, שרת ההרשאות מחזיר תגובת שגיאה.

שרת ההרשאות מגיב באמצעות קוד שגיאה וכולל את פרמטר **השגיאה** הבא בתגובה:

`invalid_request: The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed.`

`invalid_client: Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method).  The authorization server MAY return an HTTP 401 (Unauthorized) status code to indicate which HTTP authentication schemes are supported.  If the client attempted to authenticate via the "Authorization" request header field, the authorization server MUST respond with an HTTP 401 (Unauthorized) status code and include the "WWW-Authenticate" response header field matching the authentication scheme used by the client.`

`invalid_grant: The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client.`

`unauthorized_client: The authenticated client is not authorized to use this authorization grant type.`

`unsupported_grant_type: The authorization grant type is not supported by the authorization server.`

`invalid_scope: The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner.`

[פתח כרטיס תמיכה](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-troubleshooting-support-howto) כדי לפתור בעיה זו.