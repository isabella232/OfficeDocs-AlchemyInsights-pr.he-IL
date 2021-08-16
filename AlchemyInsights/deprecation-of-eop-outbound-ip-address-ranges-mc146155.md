---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031263"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>ביטול פחת של טווחי כתובות IP יוצאות של EOP

זיהינו בעיה פוטנציאלית בארגון שלך אשר (אם לא תוקנה עד ה- 26 באוקטובר 2018) עשויה לשבור את זרימת הדואר ליעדים המקומיים או החיצוניים שלך. כפי שהעברת בעבר, כדי לפשט את ניהול טווח כתובות ה- IP, אנו מאחדים את טווחי כתובות ה- IP של Exchange Online Protection (EOP) המשמשים לשליחה וקבלה של דואר אלקטרוני מחוץ Microsoft 365. הניתוח שלנו מציין שאחד או יותר ממקורות הדואר האלקטרוני או היעדים החיצוניים שתצורתם נקבעה במחברי זרימת דואר אינם מקבלים חיבורים מטווחי כתובות ה- IP המוצגים [כאן.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

פעל לפני ה- 26 באוקטובר כדי להבטיח שמקורות ויעדים אלה יקבלו חיבורים אל כל כתובות ה- IP שפורסמו [ב- EOP ומתוכן.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

לקבלת מידע נוסף אודות שינוי זה, ראה הודעות מרכז [ההודעות MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)או [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**הערה**: אם השתמשת בעבר בפרסום IP או כתובת URL באמצעות HTML , XML ו- RSS עבור עדכוני נקודות קצה, עליך גם לעבור לשירותי האינטרנט החדשים כדי להפוך עדכונים מסוגים אלה לאוטומטיים. לקבלת מידע נוסף, [ראה Microsoft 365 נקודות קצה וכתובות Microsoft 365 IP](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)ושירות אינטרנט של כתובת URL .
