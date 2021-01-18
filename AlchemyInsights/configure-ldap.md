---
title: קביעת התצורה של LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885161"
---
# <a name="configure-ldap"></a>קביעת התצורה של LDAP

כדי לקבוע את תצורת LDAP, בצע את הפעולות הבאות:

1. בדוק את תקינות התחום שלך [בפורטל התכלת](https://aka.ms/aadds-health).
1. ודא שמנוי חוקי של תכלת לספירה זמין ושירותי התחום של תכלת AD הופעלו.
1. יש לקבל את האישור הנדרש להפיכת LDAP מאובטחת מרשות אישורים ציבורית מהימנה או להיות אישור בחתימה עצמית.
1. ודא שהאישור עוקב אחר [הקווים המנחים](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)הדרושים.

**אישור לא חוקי**
1. כדי לחדש אישור, בצע את השלבים ליצירת אישור חדש והעלאה מחדש: [קביעת התצורה של LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. כדי לפתור בעיה ידועה באמצעות התראות LDAP מאובטחות בשירותי התחום של Active directory, ראה [פתרון התראות של ldap](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
