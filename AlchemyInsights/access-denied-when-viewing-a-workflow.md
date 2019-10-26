---
title: הגישה נדחתה בעת הצגת זרימת עבודה
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747749"
---
# <a name="access-denied-when-viewing-a-workflow"></a>הגישה נדחתה בעת הצגת זרימת עבודה

SharePoint 2013 זרימות עבודה שמנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint יכולה להיכשל בהודעת שגיאה "הגישה נדחתה" אם החברות בקבוצת SharePoint אינה מוגדרת ככולם.
  
 **כדי לפתור בעיה זו, בצע את הפעולות הבאות:**
  
 1. אפשר לכולם לראות את החברים בקבוצת SharePoint.
  
 2. הסר את קבוצת SharePoint מהשורה ' אל ' או ' עותק ' של הדואר האלקטרוני.
  
 3. הוסף במפורש את המשתמשים לשורה ' אל ' או ' עותק ' אם אין אפשרות לשנות את ניראות החברות עבור קבוצת SharePoint.
  
כדי לצפות בפרטים נוספים, עיין ב- [HTTP לא מורשה ל-/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  