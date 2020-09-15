---
title: 1554 Winsock error 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698863"
---
# <a name="winsock-error-10061"></a>Winsock error 10061

קוד שגיאה זה מציין ש-Microsoft לא הצליח ליצור שקע TCP (חיבור) עם מארח היעד. הגורם הסביר ביותר לשגיאה זו הוא בעיה בתצורת חומת האש שלך. כדי לפתור את הבעיה, בדוק הגדרות אלה:

- אימות תצורת חומת האש עם המידע [בכתובות url וטווחי כתובות IP של Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- אם השגיאה ספציפית ל-Exchange Online Protection (EOP), היית אמור לקבל הודעה בעבר על שינוי [בכתובות ה-IP של Exchange Online protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- ודא שספק שירותי האינטרנט (ISP) שלך אינו חוסם את היציאה.

- אמת את הגדרות שרת המארח החכם ושרת היעד במחברים.

שים לב ש-Microsoft 365 אינו חוסם חיבורים *נכנסים* באופן זה.
