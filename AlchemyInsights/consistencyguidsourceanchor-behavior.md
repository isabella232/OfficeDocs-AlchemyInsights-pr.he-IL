---
title: התנהגות ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756284"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>התנהגות ConsistencyGuid/sourceAnchor

התחברות למודעת תכלת (גירסה 1.1.524.0 ואחרי) מסייעת כעת לשימוש ב-msDS-ConsistencyGuid כתכונה sourceAnchor. בעת שימוש בתכונה זו, התכונה ' תכלת לספירה ' מגדירה באופן אוטומטי את כללי הסינכרון ל:
  
- השתמש ב-msDS-ConsistencyGuid כתכונה של sourceAnchor עבור אובייקטי משתמשים. ObjectGUID משמש עבור סוגי אובייקטים אחרים.
    
- עבור כל אובייקט מקומי נתון של AD מקומי שהתכונה msDS-ConsistencyGuid אינה מאוכלסת, הקישור תכלת AD כותב את ערך objectGUID בחזרה לתכונה msDS-ConsistencyGuid ב-Active Directory מקומי. לאחר שהתכונה msDS-ConsistencyGuid מאוכלסת, האפשרות תכלת AD Connect ולאחר מכן מייצאת את האובייקט לכיוון תכלת לספירה.
    
 **הערה:** לאחר הייבוא של אובייקט AD מקומי לחיבור הודעות מיידיות (כלומר, המיובא לשטח מחבר המודעה ומוקרן לתוך Metaverse), אין באפשרותך לשנות את הערך של sourceAnchor עוד. כדי לציין את הערך של sourceAnchor עבור אובייקט AD מקומי נתון, קבע את תצורת התכונה msDS-ConsistencyGuid לפני הייבוא לתוך הקישור תכלת AD. 
  
לקבלת מידע נוסף אודות SourceAnchor ו-ConsistencyGuid, עיין במאמר הבא: [מושגי החיבור של תכלת לספירה: מושגי עיצוב](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

