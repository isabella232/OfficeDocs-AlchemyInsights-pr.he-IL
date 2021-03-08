---
title: הקצאת תפקיד ביומן ביקורת במרכז התאימות & אבטחה של Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524793"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="41b43-102">הקצאת תפקיד ביומן ביקורת במרכז התאימות & אבטחה של Office 365</span><span class="sxs-lookup"><span data-stu-id="41b43-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="41b43-103">כדי לחפש ביומן הביקורת של Office 365, יש להקצות למנהל מערכת **ביקורת בלבד** או תפקיד **יומני ביקורת** ב-Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="41b43-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="41b43-104">תפקידים אלה מוקצים לקבוצות התפקידים ניהול תאימות וניהול ארגון כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="41b43-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="41b43-105">מנהלי מערכת כלליים ב-Office 365 ו-Microsoft 365 נוספים באופן אוטומטי כחברים בקבוצת התפקידים ' ניהול ארגון '.</span><span class="sxs-lookup"><span data-stu-id="41b43-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="41b43-106">כדי לאפשר למשתמש לחפש ברמה המינימלית של הרשאות, צור קבוצת תפקידים מותאמת אישית ב-Exchange Online, הוסף את תפקיד **יומני הביקורת לתצוגה בלבד** או תפקיד **יומני ביקורת** , ולאחר מכן הוסף את המשתמש כחבר בקבוצת התפקידים החדשה.</span><span class="sxs-lookup"><span data-stu-id="41b43-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="41b43-107">לקבלת מידע נוסף, ראה [ניהול קבוצות תפקידים ב-Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) [וחיפוש ביומן הביקורת במרכז התאימות של אבטחה &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="41b43-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>