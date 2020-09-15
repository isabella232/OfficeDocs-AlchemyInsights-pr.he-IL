---
title: ATP עבור SharePoint, OneDrive ו-Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715562"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="753c8-102">ATP עבור SharePoint, OneDrive ו-Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="753c8-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="753c8-103">בצע שלבים אלה כדי לאפשר הגנה מתקדמת של איום:</span><span class="sxs-lookup"><span data-stu-id="753c8-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="753c8-104">עבור אל [https://protection.office.com](https://protection.office.com) והיכנס באמצעות חשבון מנהל מערכת כללי או מנהל אבטחה.</span><span class="sxs-lookup"><span data-stu-id="753c8-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="753c8-105">בחלונית הניווט הימנית תחת **ניהול האיום**, בחר באפשרות קבצים מצורפים בטוחים **של מדיניות** \> **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="753c8-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="753c8-106">בחר **הפעל את ATP עבור SharePoint, OneDrive ו-Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="753c8-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="753c8-107">[צור מדיניות התראת פעילות](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) כדי לקבל הודעות כאשר אנו מזהים קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="753c8-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="753c8-108">לקבלת הוראות מלאות, עיין [בנושא](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)זה.</span><span class="sxs-lookup"><span data-stu-id="753c8-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="753c8-109">**הערה**: לפי עיצוב, ATP אינו סורק כל קובץ בודד ב-SharePoint Online, ב-OneDrive for Business או ב-Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="753c8-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="753c8-110">הקבצים נסרקים באופן אסינכרוני על-ידי תהליך המשתמש בפעילות שיתוף, בפעילות אורחת ובאותות איום כדי לזהות קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="753c8-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="753c8-111">לקבלת מידע נוסף, עיין [בנושא](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)זה.</span><span class="sxs-lookup"><span data-stu-id="753c8-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
