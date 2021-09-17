---
title: תמונת המשתמש עדיין מופיעה בתרשים Microsoft Teams הארגוני
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422253"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>תמונת המשתמש עדיין מופיעה בתרשים Microsoft Teams הארגוני

אם אדם אחד או יותר בארגון שלך הפך ללא זמין או הוסר, ותמונת הפרופיל שלו עדיין מופיעה בתרשים הארגוני, ייתכן שההגדרה **ShowInAddressLists** מוגדרת כ- False: 

1. עבור אל מרכז הניהול של Microsoft 365 > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) ובחר את המשתמש עם התמונה שעדיין מופיעה. 
1. בחר את **הכרטיסיה דואר** ולאחר מכן ודא **שהרשימה הצג ברשימת כתובות כללית** מוגדרת ללא . 

אם הגדרת **ShowInAddressLists** **ל'לא'** אינה פועלים, בדוק את הפעולות הבאות: 

- המשתמש עשוי להיות מוצג מרשימת הנמענים Exchange. לקבלת מידע נוסף, ראה [ניהול רשימות כתובות ב- Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- ייתכן שהמשתמש יוצג מרשימת הכתובות ב- Azure Active Directory. לקבלת מידע נוסף, ראה [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 