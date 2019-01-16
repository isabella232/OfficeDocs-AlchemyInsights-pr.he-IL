---
title: שגיאת Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292017"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="5d27e-102">שגיאת Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="5d27e-102">Winsock error 10061</span></span>

<span data-ttu-id="5d27e-p101">קוד שגיאה זו פירושה כי Office 365 לא היתה אפשרות ליצור שקע TCP (חיבור) עם מארח היעד. הסיבה הסבירה ביותר לשגיאה זו היא בעיה בתצורת חומת האש שלך. כדי לפתור את הבעיה, בדוק את הגדרות אלה:</span><span class="sxs-lookup"><span data-stu-id="5d27e-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="5d27e-106">ודא את תצורת חומת האש שלך עם המידע ב- [Office 365 Url ואת טווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="5d27e-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="5d27e-107">אם השגיאה הוא ספציפי כדי Exchange Online הגנה (EOP), יש קיבלת בעבר הודעה על שינוי [כתובות IP הגנה מקוונת של Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5d27e-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="5d27e-108">ודא כי את ספק שירותי האינטרנט (ISP) אינה חוסמת את היציאה.</span><span class="sxs-lookup"><span data-stu-id="5d27e-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="5d27e-109">אמת את חכמה מארח והיעד הגדרות השרת במחברים שלך.</span><span class="sxs-lookup"><span data-stu-id="5d27e-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="5d27e-110">שים לב כי Office 365 לא תחסום חיבורים *נכנסים* באופן זה.</span><span class="sxs-lookup"><span data-stu-id="5d27e-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

