---
title: בעיה בהצטרפות לוירטואלית
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885210"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="634f8-102">בעיה בהצטרפות לוירטואלית</span><span class="sxs-lookup"><span data-stu-id="634f8-102">Issue joining VMs</span></span>

<span data-ttu-id="634f8-103">כדי לפתור בעיות המתרחשות בעת ניסיון להצטרף ל-וירטואלית, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="634f8-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="634f8-104">נסה להיכנס באמצעות תבנית **UPN** (לדוגמה, ' joeuser@contoso.com ') במקום בתבנית **SAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="634f8-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="634f8-105">ודא שהפעלת סינכרון סיסמאות בהתאם לשלבים *המתוארים במדריך תחילת* העבודה.</span><span class="sxs-lookup"><span data-stu-id="634f8-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="634f8-106">ודא שחשבון המשתמש המושפע אינו חשבון חיצוני בדייר תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="634f8-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="634f8-107">משתמשים חיצוניים אינם יכולים להיכנס לתחום המנוהל מאחר ששירותי התחום של תכלת AD אינם כוללים אישורים עבור חשבונות משתמשים אלה.</span><span class="sxs-lookup"><span data-stu-id="634f8-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="634f8-108">אם חשבון המשתמש המושפע הוא חשבון משתמש בענן בלבד, ודא שהמשתמשים החליפו את הסיסמה שלהם לאחר הפעלת שירותים בתחום התכלת של AD.</span><span class="sxs-lookup"><span data-stu-id="634f8-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="634f8-109">שלב זה גורם לפעולות ה-hash של האישורים הדרושים עבור שירותי התחום של תכלת AD ליצירה.</span><span class="sxs-lookup"><span data-stu-id="634f8-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="634f8-110">אם חשבונות המשתמשים המושפעים מסונכרנים מתוך מדריך כתובות מקומי, ודא שתצורת ההפצה המומלצת של התחברות התכלת של התכלת הוגדרה לביצוע סינכרון מלא.</span><span class="sxs-lookup"><span data-stu-id="634f8-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="634f8-111">אם הבעיות נמשכות לאחר אישור שלב 4, הפעל את הפקודות הבאות מתוך מחשב הסינכרון:</span><span class="sxs-lookup"><span data-stu-id="634f8-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="634f8-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="634f8-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>