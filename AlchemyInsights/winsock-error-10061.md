---
title: שגיאת Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772443"
---
# <a name="winsock-error-10061"></a>שגיאת Winsock 10061

קוד שגיאה זו פירושה כי Office 365 לא היתה אפשרות ליצור שקע TCP (חיבור) עם מארח היעד. הסיבה הסבירה ביותר לשגיאה זו היא בעיה בתצורת חומת האש שלך. כדי לפתור את הבעיה, בדוק את הגדרות אלה:
  
- ודא את תצורת חומת האש שלך עם המידע ב- [Office 365 Url ואת טווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- אם השגיאה הוא ספציפי כדי Exchange Online הגנה (EOP), יש קיבלת בעבר הודעה על שינוי [כתובות IP הגנה מקוונת של Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- ודא כי את ספק שירותי האינטרנט (ISP) אינה חוסמת את היציאה.
    
- אמת את חכמה מארח והיעד הגדרות השרת במחברים שלך.
    
שים לב כי Office 365 לא תחסום חיבורים *נכנסים* באופן זה. 
  

