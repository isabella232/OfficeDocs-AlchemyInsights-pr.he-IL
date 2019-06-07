---
title: 1065 הביטול של IP יוצאת EOP לטפל rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752956"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>הביטול של טווחי כתובות ה-IP יוצאת EOP

אנו כבר זיהה בעיה פוטנציאלית עם הארגון שלך (אם לא תתוקן על-ידי ה-26 באוקטובר, 2018) עלול להפר זרימת דואר מקומיות או ליעדים חיצוניים. כמו בעבר communicated, כדי לפשט את ניהול טווח של כתובות IP, אנו האיחוד טווחי כתובות IP Exchange Online הגנה (EOP) בהם נעשה שימוש כדי לשלוח ולקבל דואר אלקטרוני מחוץ ל- Office 365. הניתוח שלנו מציין כי אחד או יותר של מקורות חיצוניים דוא ל או ליעדים שקבעת במחברים זרימת דואר אינם קבלת חיבורים IP כתובת טווחים המוצגת [כאן](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

לפעול לפני אוקטובר ה-26 שתבטיח שמקורות ויעדים אלה יקבל חיבורים בין כל [פרסום כתובות EOP IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

לקבלת מידע נוסף אודות שינוי זה, נא עיין שבמרכז הודעה הצבות [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)או [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**הערה**: אם השתמשת בעבר פרסום כתובת IP או כתובת URL באמצעות HTML, XML ו- RSS עבור נקודת הקצה של עדכונים, אתה גם צריך להעביר לשירותי אינטרנט חדש לאוטומציה של סוגים אלה של עדכונים. לקבלת מידע נוסף, ראה [קטגוריות קצה של Office 365 ואת כתובת ה-IP של Office 365 כתובת URL של שירות האינטרנט](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
