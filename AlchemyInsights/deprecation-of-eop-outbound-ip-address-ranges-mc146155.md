---
title: 1065 הדיון של כתובת IP יוצאת של EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704598"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="c0b03-102">הדיון של טווחי כתובות IP יוצאות של EOP</span><span class="sxs-lookup"><span data-stu-id="c0b03-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="c0b03-103">גילינו בעיה פוטנציאלית עם הארגון שלך (אם לא תוקן עד ה -26 באוקטובר, 2018) עלול לשבור את זרימת הדואר אל היעדים המקומיים או החיצוניים שלך.</span><span class="sxs-lookup"><span data-stu-id="c0b03-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="c0b03-104">כפי שמועבר קודם לכן, כדי לפשט את ניהול טווח כתובות ה-IP, אנו מאחדים את טווחי כתובות ה-IP של Exchange Online (EOP) המשמשים לשליחה וקבלה של דואר אלקטרוני מחוץ ל-Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c0b03-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="c0b03-105">הניתוח שלנו מצביע על כך שאחד או יותר ממקורות הדואר האלקטרוני או היעדים החיצוניים שהגדרת במחברי זרימת הדואר אינם מקבלים חיבורים מטווחי כתובות ה-IP המוצגים [כאן](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c0b03-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c0b03-106">לפעול לפני ה -26 באוקטובר כדי להבטיח שמקורות ויעדים אלה יקבלו התקשרויות אל ומכל [כתובות ה-EOP המתפרסמות שפורסמו](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c0b03-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c0b03-107">לקבלת מידע נוסף אודות שינוי זה, ראה מרכז הודעות הודעות [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)או [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="c0b03-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="c0b03-108">**הערה**: אם השתמשת בעבר בפרסום IP או URL באמצעות HTML, XML ו-RSS עבור עדכוני נקודות קצה, עליך גם לעבור לשירותי האינטרנט החדשים לאוטומציה של סוגי עדכונים אלה.</span><span class="sxs-lookup"><span data-stu-id="c0b03-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="c0b03-109">לקבלת מידע נוסף, ראה [קטגוריות נקודות קצה של microsoft 365 ו-microsoft 365 כתובת IP ושירות אינטרנט של כתובות URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="c0b03-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
