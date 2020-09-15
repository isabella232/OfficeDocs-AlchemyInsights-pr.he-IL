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
# <a name="winsock-error-10061"></a><span data-ttu-id="c1527-102">Winsock error 10061</span><span class="sxs-lookup"><span data-stu-id="c1527-102">Winsock error 10061</span></span>

<span data-ttu-id="c1527-103">קוד שגיאה זה מציין ש-Microsoft לא הצליח ליצור שקע TCP (חיבור) עם מארח היעד.</span><span class="sxs-lookup"><span data-stu-id="c1527-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c1527-104">הגורם הסביר ביותר לשגיאה זו הוא בעיה בתצורת חומת האש שלך.</span><span class="sxs-lookup"><span data-stu-id="c1527-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c1527-105">כדי לפתור את הבעיה, בדוק הגדרות אלה:</span><span class="sxs-lookup"><span data-stu-id="c1527-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="c1527-106">אימות תצורת חומת האש עם המידע [בכתובות url וטווחי כתובות IP של Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c1527-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="c1527-107">אם השגיאה ספציפית ל-Exchange Online Protection (EOP), היית אמור לקבל הודעה בעבר על שינוי [בכתובות ה-IP של Exchange Online protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c1527-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="c1527-108">ודא שספק שירותי האינטרנט (ISP) שלך אינו חוסם את היציאה.</span><span class="sxs-lookup"><span data-stu-id="c1527-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="c1527-109">אמת את הגדרות שרת המארח החכם ושרת היעד במחברים.</span><span class="sxs-lookup"><span data-stu-id="c1527-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="c1527-110">שים לב ש-Microsoft 365 אינו חוסם חיבורים *נכנסים* באופן זה.</span><span class="sxs-lookup"><span data-stu-id="c1527-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
