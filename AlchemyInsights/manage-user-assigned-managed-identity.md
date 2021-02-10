---
title: ניהול זהות מנוהלת שהוקצתה על-ידי המשתמש
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
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177579"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="8bbf0-102">ניהול זהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="8bbf0-103">הניהול של זהות מנוהלת שהוקצתה על-ידי המשתמש כרוך:</span><span class="sxs-lookup"><span data-stu-id="8bbf0-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="8bbf0-104">הקצאת תפקידים לזהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="8bbf0-105">מחיקת זהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="8bbf0-106">רישום זהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="8bbf0-107">לקבלת מידע נוסף אודות המשימות שהוזכרו לעיל, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="8bbf0-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="8bbf0-108">[כיצד ליצור זהות מנוהלת שהוקצתה](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) על-ידי המשתמש-עבור הקצאת תפקידים לזהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="8bbf0-109">[כיצד למחוק זהות מנוהלת שהוקצתה](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) על-ידי המשתמש-למחיקת זהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="8bbf0-110">[כיצד להציג רשימה של זהות מנוהלת שהוקצתה](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) על-ידי המשתמש-לרישום זהות מנוהלת שהוקצתה על-ידי המשתמש</span><span class="sxs-lookup"><span data-stu-id="8bbf0-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="8bbf0-111">בדיקה אם יש לך את הקצאת התפקידים ' **משתתף בניהול זהויות** '.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="8bbf0-112">הקצאת תפקיד זו נדרשת ליצירה/מחיקה של זהויות מנוהלות שהוקצו על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="8bbf0-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
