---
title: Access נדחתה בעת הצגת זרימת עבודה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955202"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access נדחתה בעת הצגת זרימת עבודה

SharePoint זרימות עבודה של Access 13 שמנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint עלולות להיכשל עם הודעת שגיאה "Access נדחתה" אם החברות בקבוצה SharePoint אינה מוגדרת ככולם.
  
 **כדי לפתור בעיה זו, בצע את הפעולות הבאות:**
  
 1. אפשר לכולם לראות את החברים בקבוצה SharePoint.
  
 2. הסר את SharePoint מהקו אל או עותק של הודעת הדואר האלקטרוני.
  
 3. הוסף את המשתמשים באופן מפורש לקו אל או ל- CC אם לא ניתן לשנות את הניראות של החברות עבור SharePoint הקבוצה.
  
כדי להציג פרטים נוספים, עיין ב- HTTP לא מורשה [ל- /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  