---
title: קביעת תצורה של LDAP
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090413"
---
# <a name="configure-ldap"></a>קביעת תצורה של LDAP

כדי לקבוע את התצורה של LDAP, עשה את הפעולות הבאות:

1. בדוק את תקינות התחום שלך בפורטל [Azure](https://aka.ms/aadds-health).
1. ודא שמנוי Azure AD חוקי זמין ושירותי Azure AD Domain Services הופעלו.
1. יש להשיג את האישור הדרוש כדי להפוך את LDAP מאובטח לזמין מרשות אישורים ציבורית מהימנה או להיות אישור בחתימה עצמית.
1. ודא שהאישור פועל לפי הקווים [המנחים הדרושים.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**אישור לא חוקי**
1. כדי לחדש אישור, בצע את השלבים ליצירת אישור חדש וטעינה מחדש: קביעת תצורה [של LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. כדי לפתור בעיה ידועה בהתראות Secure LDAP ב- Azure Active directory Domain Services, ראה [פתרון התראות LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
