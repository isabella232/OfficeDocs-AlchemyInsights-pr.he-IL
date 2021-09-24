---
title: שינוי משרתי השמות של Microsoft בחזרה לניהול רשומות DNS משלך
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506604"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>שינוי משרתי השמות של Microsoft בחזרה לניהול רשומות DNS משלך

שינית בעבר את רשומות ה- NS כדי להצביע על Microsoft (ns1.bdm.microsoftonline.com) אך החלטת כעת לנהל רשומות DNS משלך:

באתר האינטרנט של רשם התחומים שלך, שנה את שירות השמות בחזרה לרשם או להגדרה הקודמת. אם אינך בקיא ב- DNS, פנה לתמיכה אצל רשם התחומים. שים לב שהפצה של שינויים של משרת השמות יכולה לאסוף עד 48 שעות. 

1. בפורטל Microsoft 365, עבור אל **הגדרות**  >  [**תחומים**](https://admin.microsoft.com/Adminportal/Home#/Domains), בחר את תיבת הסימון לצד התחום ובחר ניהול **DNS**. 

2. באשף, בחר הוסף **רשומות DNS משלך והשלם** את האשף. פעולה זו משנה את אופן הניהול של ה- DNS ולאחר מכן מאפשרת לך להוסיף את רשומות ה- DNS המותאמות אישית הדרושות כדי לתמוך בשירותים שנבחרו.

לחלופין, אם שינית את רשומות שרת השמות שלך ל- Microsoft ויש לך אתר אינטרנט, באפשרותך להוסיף רשומות DNS עבור אתר האינטרנט במקום לשנות את שרתי השמות בחזרה. לקבלת מידע נוסף, ראה [עדכון רשומות DNS כדי לשמור את אתר האינטרנט שלך עם ספק האירוח הנוכחי שלך.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


