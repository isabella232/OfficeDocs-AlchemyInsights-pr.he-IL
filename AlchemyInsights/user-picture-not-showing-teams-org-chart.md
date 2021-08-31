---
title: תמונת משתמש אינה מוצגת בתרשים Microsoft Teams ארגוני
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792755"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>תמונת משתמש אינה מוצגת בתרשים Microsoft Teams ארגוני

אם אדם אחד או יותר בארגון שלך חסר את תמונת הפרופיל שלו בתרשים הארגוני, ייתכן שההגדרה **ShowInAddressLists** מוגדרת ל- **False**:

1. עבור אל מרכז הניהול של Microsoft 365 > [**Active Users**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)ובחר את המשתמש עם התמונה החסרה. 
1. בחר את **הכרטיסיה דואר** ולאחר מכן ודא **ש'הצג ברשימת הכתובות הכללית'** מוגדר **כ'כן'.** 

אם הגדרת **ShowInAddressLists** **ל'כן'** אינה פועלים, בדוק את הפעולות הבאות:

- ייתכן שהמשתמש מוסתר מרשימת הנמענים Exchange. לקבלת מידע נוסף, ראה [ניהול רשימות כתובות ב- Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- ייתכן שהמשתמש מוסתר מרשימת הכתובות ב- Azure Active Directory. לקבלת מידע נוסף, ראה [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
