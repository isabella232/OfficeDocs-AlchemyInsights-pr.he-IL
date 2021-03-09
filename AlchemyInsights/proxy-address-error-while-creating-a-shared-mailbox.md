---
title: שגיאת כתובת Proxy בעת יצירת תיבת דואר משותפת
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568291"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="7f2d4-102">שגיאת כתובת Proxy בעת יצירת תיבת דואר או אובייקט אחר המותאם לשימוש בדואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="7f2d4-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="7f2d4-103">אם ניסית ליצור אובייקט המותאם לשימוש בדואר אלקטרוני (תיבת דואר, תיבת דואר משותפת וכו ') וקיבלת את השגיאה "כתובת ה-proxy" SMTP:alias@domain.com "כבר נמצאת בשימוש...", כתובת הדואר האלקטרוני שבחרת כבר נלקחה על-ידי אובייקט אחר המותאם באמצעות דואר אלקטרוני בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="7f2d4-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="7f2d4-104">עליך למצוא את המשתמש, הקבוצה, תיבת הדואר המשותפת או התיקיה הציבורית המכילה את כתובת הדואר האלקטרוני ולמחוק אותה או לשנות את כתובת הדואר האלקטרוני שלה.</span><span class="sxs-lookup"><span data-stu-id="7f2d4-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="7f2d4-105">לאחר מכן תוכל ליצור אובייקט חדש המותאם באמצעות דואר אלקטרוני עם כתובת הדואר האלקטרוני המשוחררת.</span><span class="sxs-lookup"><span data-stu-id="7f2d4-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="7f2d4-106">השתמש בחיפוש בדף הבית כדי למצוא אותו.</span><span class="sxs-lookup"><span data-stu-id="7f2d4-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="7f2d4-107">באפשרותך גם להשתמש בפקודה הבאה של Exchange Online PowerShell כדי לחפש אותו:</span><span class="sxs-lookup"><span data-stu-id="7f2d4-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="7f2d4-108">אם אינך מעוניין למחוק את כתובת הדואר האלקטרוני הקיימת, בחר כתובת דואר אלקטרוני חדשה עבור האובייקט החדש שאתה יוצר.</span><span class="sxs-lookup"><span data-stu-id="7f2d4-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  