---
title: הגישה נדחתה בעת הצגת זרימת עבודה
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050526"
---
# <a name="access-denied-when-viewing-a-workflow"></a>הגישה נדחתה בעת הצגת זרימת עבודה

SharePoint 2013 זרימות עבודה שמנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint יכולה להיכשל בהודעת שגיאה "הגישה נדחתה" אם החברות בקבוצת SharePoint אינה מוגדרת ככולם.
  
 **כדי לפתור בעיה זו, בצע את הפעולות הבאות:**
  
 1. אפשר לכולם לראות את החברים בקבוצת SharePoint.
  
 2. הסר את קבוצת SharePoint מהשורה ' אל ' או ' עותק ' של הדואר האלקטרוני.
  
 3. הוסף במפורש את המשתמשים לשורה ' אל ' או ' עותק ' אם אין אפשרות לשנות את ניראות החברות עבור קבוצת SharePoint.
  
כדי לצפות בפרטים נוספים, עיין ב- [HTTP לא מורשה ל/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  