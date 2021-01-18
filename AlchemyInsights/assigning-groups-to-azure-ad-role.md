---
title: הקצאת קבוצות לחלק התכלת לספירה
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885067"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="6c7eb-102">הקצאת קבוצות לחלק התכלת לספירה</span><span class="sxs-lookup"><span data-stu-id="6c7eb-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="6c7eb-103">כדי להקצות קבוצת מודעות של תכלת באמצעות מקור הסמכות בתכלת לספירה לתפקיד תכלת לספירה, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="6c7eb-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="6c7eb-104">צור קבוצה חדשה-כדי ליצור קבוצה חדשה:</span><span class="sxs-lookup"><span data-stu-id="6c7eb-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="6c7eb-105">מ.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-105">a.</span></span> <span data-ttu-id="6c7eb-106">היכנס למרכז הניהול של תכלת לספירה עם הרשאות **מנהל תפקידים מורשה** או **מנהל מערכת כללי** .</span><span class="sxs-lookup"><span data-stu-id="6c7eb-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="6c7eb-107">b.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-107">b.</span></span> <span data-ttu-id="6c7eb-108">בחר **באפשרות תכלת Active Directory > קבוצות > כל הקבוצות > קבוצה חדשה**.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="6c7eb-109">c.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-109">c.</span></span> <span data-ttu-id="6c7eb-110">יצירת הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-110">Create the group.</span></span>

2. <span data-ttu-id="6c7eb-111">הקצה את התפקיד לקבוצה במהלך יצירת הקבוצה או לאחר יצירת הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="6c7eb-112">מ.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-112">a.</span></span> <span data-ttu-id="6c7eb-113">כדי להקצות תפקיד לקבוצה בזמן יצירת הקבוצה, עבור לקבוצה החלפת תפקידים של העברת **הודעות מיידיות של תכלת** ויצירת הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="6c7eb-114">b.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-114">b.</span></span> <span data-ttu-id="6c7eb-115">כדי להקצות תפקיד לקבוצה לאחר יצירתה, נווט אל הכרטיסיה **תפקידים שהוקצו** עבור הקבוצה החדשה שנוצרה, והקצה את התפקיד לקבוצה.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="6c7eb-116">**ניהול חברות בקבוצה המוקצית לתפקיד ' הודעות מיידיות '**</span><span class="sxs-lookup"><span data-stu-id="6c7eb-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="6c7eb-117">כדי למנוע העלאת הרשאות, כברירת מחדל, רק מנהלי תפקידים מורשים ומנהלי מערכת כלליים יכולים לשנות את החברות של קבוצה המוקצית לתפקיד.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="6c7eb-118">עם זאת, הם יכולים לבחור להקצות בעלים עבור קבוצה כזו ולהקצות משימה זו.</span><span class="sxs-lookup"><span data-stu-id="6c7eb-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="6c7eb-119">לקבלת פרטים נוספים על הקצאת קבוצות ענן לתפקידים של הודעות מיידיות, ראה [הקצאת תפקידי פרסום לקבוצת ענן](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="6c7eb-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="6c7eb-120">לקבלת פרטים נוספים אודות פתרון בעיות המוקצות לקבוצות ענן, ראה [פתרון בעיות של תפקידים שהוקצו לקבוצות ענן](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="6c7eb-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





