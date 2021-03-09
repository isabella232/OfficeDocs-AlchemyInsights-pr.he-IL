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
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>שגיאת כתובת Proxy בעת יצירת תיבת דואר או אובייקט אחר המותאם לשימוש בדואר אלקטרוני

אם ניסית ליצור אובייקט המותאם לשימוש בדואר אלקטרוני (תיבת דואר, תיבת דואר משותפת וכו ') וקיבלת את השגיאה "כתובת ה-proxy" SMTP:alias@domain.com "כבר נמצאת בשימוש...", כתובת הדואר האלקטרוני שבחרת כבר נלקחה על-ידי אובייקט אחר המותאם באמצעות דואר אלקטרוני בארגון שלך.
  
עליך למצוא את המשתמש, הקבוצה, תיבת הדואר המשותפת או התיקיה הציבורית המכילה את כתובת הדואר האלקטרוני ולמחוק אותה או לשנות את כתובת הדואר האלקטרוני שלה. לאחר מכן תוכל ליצור אובייקט חדש המותאם באמצעות דואר אלקטרוני עם כתובת הדואר האלקטרוני המשוחררת. השתמש בחיפוש בדף הבית כדי למצוא אותו. באפשרותך גם להשתמש בפקודה הבאה של Exchange Online PowerShell כדי לחפש אותו:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
אם אינך מעוניין למחוק את כתובת הדואר האלקטרוני הקיימת, בחר כתובת דואר אלקטרוני חדשה עבור האובייקט החדש שאתה יוצר.
  