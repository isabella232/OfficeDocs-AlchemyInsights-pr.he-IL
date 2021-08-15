---
title: אבחון עבור בעיות גישה ליציאות שונות
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030903"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>אבחון עבור בעיות גישה ליציאות שונות

כדי לפתור את הבעיות השונות בגישה ליציאות, בצע את השלבים הבאים:

1. עצור/מקם את המחשב הווירטואלי (VM) מהפורטל, הפעל מחדש את ה- VM ולאחר מכן מחשב שוב. 
2. בדוק את הגדרות הרשת של VM כדי לקבוע אם יש לך קבוצות אבטחת רשת (NSG) שחוסמות את התעבורה. באפשרותך גם להשתמש בכלי אימות זרימת [ה- IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) של צופה הרשת כדי לבדוק אם תעבורה חסימת NSG, ניתובי User-Defined (UDRs) מנתבים מחדש את התעבורה שלך בחזרה לסביבה המקומית ('מסלול ברירת מחדל' 0.0.0.0/0) או אל מכשיר רשת.
אם אתה עדיין נתקל בבעיות לאחר שניסית את השלבים לעיל, ספק את שם ה- VM ואת יציאת ה- TCP שאתה מנסה לשלוח בה דואר לקבלת אבחון נוסף.

**מסמכים מומלצים**

[מגבלות והמלצות לשליחת דואר אלקטרוני יוצא דרך יציאה 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)