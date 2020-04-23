---
title: 1554 Winsock שגיאה 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766170"
---
# <a name="winsock-error-10061"></a>Winsock שגיאה 10061

קוד שגיאה זה משמעו ש-Microsoft לא הצליחה ליצור שקע TCP (חיבור) עם מחשב המארח המיועד. הסיבה הסבירה ביותר לשגיאה זו היא בעיה בתצורת חומת האש שלך. כדי לפתור את הבעיה, בדוק הגדרות אלה:

- אמת את תצורת חומת האש שלך עם המידע [בכתובות Url של Microsoft 365 ובטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- אם השגיאה היא ספציפית ל-Exchange Online הגנה (EOP), היה עליך לקבל הודעה בעבר לשינוי [בכתובות ה-IP של הגנת Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- ודא שספק שירותי האינטרנט (ISP) אינו חוסם את היציאה.

- אמת את הגדרות המחשב המארח החכם ושרת היעד במחברים.

שים לב ש-Microsoft 365 אינו חוסם חיבורים *נכנסים* באופן זה.
