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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>הדיון של טווחי כתובות IP יוצאות של EOP

גילינו בעיה פוטנציאלית עם הארגון שלך (אם לא תוקן עד ה -26 באוקטובר, 2018) עלול לשבור את זרימת הדואר אל היעדים המקומיים או החיצוניים שלך. כפי שמועבר קודם לכן, כדי לפשט את ניהול טווח כתובות ה-IP, אנו מאחדים את טווחי כתובות ה-IP של Exchange Online (EOP) המשמשים לשליחה וקבלה של דואר אלקטרוני מחוץ ל-Microsoft 365. הניתוח שלנו מצביע על כך שאחד או יותר ממקורות הדואר האלקטרוני או היעדים החיצוניים שהגדרת במחברי זרימת הדואר אינם מקבלים חיבורים מטווחי כתובות ה-IP המוצגים [כאן](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

לפעול לפני ה -26 באוקטובר כדי להבטיח שמקורות ויעדים אלה יקבלו התקשרויות אל ומכל [כתובות ה-EOP המתפרסמות שפורסמו](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

לקבלת מידע נוסף אודות שינוי זה, ראה מרכז הודעות הודעות [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)או [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**הערה**: אם השתמשת בעבר בפרסום IP או URL באמצעות HTML, XML ו-RSS עבור עדכוני נקודות קצה, עליך גם לעבור לשירותי האינטרנט החדשים לאוטומציה של סוגי עדכונים אלה. לקבלת מידע נוסף, ראה [קטגוריות נקודות קצה של microsoft 365 ו-microsoft 365 כתובת IP ושירות אינטרנט של כתובות URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
