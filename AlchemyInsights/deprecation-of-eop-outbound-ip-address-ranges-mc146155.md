---
title: 1065 הביטול של IP יוצאת EOP לטפל rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777273"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="ddbff-102">הביטול של טווחי כתובות ה-IP יוצאת EOP</span><span class="sxs-lookup"><span data-stu-id="ddbff-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="ddbff-103">אנו כבר זיהה בעיה פוטנציאלית עם הארגון שלך (אם לא תתוקן על-ידי ה-26 באוקטובר, 2018) עלול להפר זרימת דואר מקומיות או ליעדים חיצוניים.</span><span class="sxs-lookup"><span data-stu-id="ddbff-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="ddbff-104">כמו בעבר communicated, כדי לפשט את ניהול טווח של כתובות IP, אנו האיחוד טווחי כתובות IP Exchange Online הגנה (EOP) בהם נעשה שימוש כדי לשלוח ולקבל דואר אלקטרוני מחוץ ל- Office 365.</span><span class="sxs-lookup"><span data-stu-id="ddbff-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="ddbff-105">הניתוח שלנו מציין כי אחד או יותר של מקורות חיצוניים דוא ל או ליעדים שקבעת במחברים זרימת דואר אינם קבלת חיבורים IP כתובת טווחים המוצגת [כאן](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ddbff-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="ddbff-106">לפעול לפני אוקטובר ה-26 שתבטיח שמקורות ויעדים אלה יקבל חיבורים בין כל [פרסום כתובות EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ddbff-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="ddbff-107">לקבלת מידע נוסף אודות שינוי זה, נא עיין שבמרכז הודעה הצבות [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)או [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="ddbff-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="ddbff-108">**הערה**: אם השתמשת בעבר פרסום כתובת IP או כתובת URL באמצעות HTML, XML ו- RSS עבור נקודת הקצה של עדכונים, אתה גם צריך להעביר לשירותי אינטרנט חדש לאוטומציה של סוגים אלה של עדכונים.</span><span class="sxs-lookup"><span data-stu-id="ddbff-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="ddbff-109">לקבלת מידע נוסף, ראה [קטגוריות קצה של Office 365 ואת כתובת ה-IP של Office 365 כתובת URL של שירות האינטרנט](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="ddbff-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

