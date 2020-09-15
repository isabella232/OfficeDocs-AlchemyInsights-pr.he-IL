---
title: Access נדחה בעת הצגת זרימת עבודה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688803"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access נדחה בעת הצגת זרימת עבודה

זרימות עבודה של SharePoint 2013 המנסות לשלוח הודעת דואר אלקטרוני לקבוצת SharePoint יכולה להיכשל עם הודעת השגיאה "הגישה נדחתה" אם החברות בקבוצת SharePoint אינה מוגדרת לכולם.
  
 **כדי לפתור בעיה זו, בצע שלבים אלה:**
  
 1. אפשר לכולם לראות את החברים בקבוצת SharePoint.
  
 2. הסר את הקבוצה של SharePoint מהשורה אל או עותק של הודעת הדואר האלקטרוני.
  
 3. הוסף את המשתמשים באופן מפורש לשורה ' אל ' או ' עותק ' אם לא ניתן לשנות את ניראות החברות עבור קבוצת SharePoint.
  
כדי להציג פרטים נוספים, עיין במאמר [HTTP לא מורשה ל/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  