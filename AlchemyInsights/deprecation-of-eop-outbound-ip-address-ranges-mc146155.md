---
title: 1065 תבטלות של EOP כתובת IP יוצאת rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806796"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>תבטלות של טווחי כתובות IP יוצאות של EOP

זיהינו בעיה אפשרית עם הארגון שלך (אם לא תוקנה על-ידי ה-26 באוקטובר, 2018) עשויה לשבור את זרימת הדואר ליעדים המקומיים או החיצוניים שלך. כאמור, כדי לפשט את ניהול טווחי כתובות ה-IP, אנו מאוחדים את טווחי כתובות ה-IP של Exchange Online Protection (EOP) המשמשים לשליחה וקבלה של דואר אלקטרוני מחוץ ל-Microsoft 365. הניתוח שלנו מציין שאחד או יותר ממקורות הדואר האלקטרוני או היעדים החיצוניים שהגדרת במחברי זרימת הדואר אינם מקבלים חיבורים מטווחי כתובות ה-IP המוצגים [כאן](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

הפעל לפני 26 באוקטובר כדי להבטיח שמקורות אלה ויעדים אלה יקבלו חיבורים לכל [כתובות ה-IP של EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

לקבלת מידע נוסף אודות שינוי זה, ראה מרכז ההודעות הודעות [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)או [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**הערה**: אם השתמשת בעבר ב-IP או בפרסום של כתובות URL באמצעות HTML, XML ו-RSS עבור עדכוני נקודות קצה, עליך גם לעבור לשירותי האינטרנט החדשים לאוטומציה של סוגי עדכונים אלה. לקבלת מידע נוסף, ראה [קטגוריות נקודות קצה של microsoft 365 ו-microsoft 365 כתובת IP ושירות אינטרנט של כתובות URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
