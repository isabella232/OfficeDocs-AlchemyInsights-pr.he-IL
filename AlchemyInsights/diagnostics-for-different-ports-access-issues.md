---
title: אבחון בעיות גישה ליציאות שונות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035783"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>אבחון בעיות גישה ליציאות שונות

כדי לפתור את בעיות הגישה ליציאות השונות, בצע את השלבים הבאים:

1. עצור/בטל את ההקצאה של המחשב הווירטואלי (VM) מתוך הפורטל, הפעל מחדש את ה-VM ובדוק שוב. 
2. בדוק את הגדרות הרשת של ה-VM שלך כדי לקבוע אם אתה מבצע חסימת תעבורה בקבוצות אבטחה של רשת (NSGs). באפשרותך גם להשתמש [בכלי אימות זרימת הזרימה של ה-IP של הצופה ברשת](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) כדי לבדוק אם קיימות תעבורה לחסימת NSGs, מסלולי User-Defined (UDRs) ניתוב מחדש של התעבורה בחזרה למכשיר המקומי (' נתיב ברירת המחדל ' ב-0.0.0.0/0) או במכשיר רשת.
אם אתה עדיין נתקל בבעיות לאחר שניסית את השלבים לעיל, ספק את שם ה-VM ואת יציאת ה-TCP שאתה מנסה לשלוח בדואר לצורך אבחון נוסף.

**מסמכים מומלצים**

[מגבלות והמלצות לשליחת דואר אלקטרוני יוצא דרך יציאה 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)