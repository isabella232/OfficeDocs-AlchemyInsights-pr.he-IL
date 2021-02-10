---
title: בעיה עם קבוצות אבטחה
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177495"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="ac973-102">בעיה עם קבוצות אבטחה</span><span class="sxs-lookup"><span data-stu-id="ac973-102">Issue with security groups</span></span>

<span data-ttu-id="ac973-103">**אם אתה מקבל את שגיאת הרשת AADDS104**</span><span class="sxs-lookup"><span data-stu-id="ac973-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="ac973-104">כללי קבוצת אבטחת רשת לא חוקיים הם הגורם הנפוץ ביותר לשגיאות רשת עבור שירותי התחום של תכלת Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="ac973-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="ac973-105">קבוצת אבטחת הרשת עבור הרשת הוירטואלית חייבת לאפשר גישה ליציאות ולפרוטוקולים ספציפיים.</span><span class="sxs-lookup"><span data-stu-id="ac973-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="ac973-106">אם יציאות אלה נחסמות, לפלטפורמת התכלת אין אפשרות לנטר או לעדכן את התחום המנוהל.</span><span class="sxs-lookup"><span data-stu-id="ac973-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="ac973-107">הסינכרון בין תכלת לספירה לבין תכלת AD DS מושפע אף הוא.</span><span class="sxs-lookup"><span data-stu-id="ac973-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="ac973-108">ודא שאתה משאיר את יציאות ברירת המחדל פתוחות כדי למנוע הפרעה בשירות.</span><span class="sxs-lookup"><span data-stu-id="ac973-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="ac973-109">כדי להבין ולפתור התראות נפוצות עבור בעיות תצורה של קבוצת אבטחת רשת, ראה [הוספה ואימות של קבוצות אבטחה](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="ac973-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
