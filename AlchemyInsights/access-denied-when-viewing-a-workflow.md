---
title: הגישה נדחתה בעת הצגת זרימת עבודה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687331"
---
# <a name="access-denied-when-viewing-a-workflow"></a>הגישה נדחתה בעת הצגת זרימת עבודה

SharePoint 2013 זרימות עבודה שמנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint יכולה להיכשל בהודעת שגיאה "הגישה נדחתה" אם החברות בקבוצת SharePoint אינה מוגדרת ככולם.
  
 **כדי לפתור בעיה זו, בצע את הפעולות הבאות:**
  
 1. אפשר לכולם לראות את החברים בקבוצת SharePoint.
  
 2. הסר את קבוצת SharePoint מהשורה ' אל ' או ' עותק ' של הדואר האלקטרוני.
  
 3. הוסף במפורש את המשתמשים לשורה ' אל ' או ' עותק ' אם אין אפשרות לשנות את ניראות החברות עבור קבוצת SharePoint.
  
כדי לצפות בפרטים נוספים, עיין ב- [HTTP לא מורשה ל/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  