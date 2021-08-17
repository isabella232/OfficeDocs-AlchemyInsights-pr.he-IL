---
title: שגיאת Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083231"
---
# <a name="winsock-error-10061"></a>שגיאת Winsock 10061

קוד שגיאה זה פירושו של- Microsoft לא היתה אפשרות ליצור שקע TCP (חיבור) עם מארח היעד. הסיבה הצפויה ביותר לשגיאה זו היא בעיה בתצורת חומת האש שלך. כדי לפתור את הבעיה, בדוק הגדרות אלה:

- אמת את תצורת חומת האש שלך עם המידע [Microsoft 365 URL וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- אם השגיאה ספציפית Exchange Online Protection (EOP), היית אמור לקבל הודעה בעבר על שינוי בכתובות [ה- IP Exchange Online Protection ה- IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- ודא שספק שירותי האינטרנט (ISP) שלך אינו חוסם את היציאה.

- אמת את הגדרות השרת המארח החכם והיעד במחברים שלך.

שים לב Microsoft 365 אינו *חוסם חיבורים* נכנסים באופן זה.
