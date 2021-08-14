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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062909"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>שגיאת כתובת Proxy בעת יצירת תיבת דואר או אובייקט אחר התאפשר בדואר אלקטרוני

אם ניסית ליצור אובייקט מותכן לדואר אלקטרוני (תיבת דואר, תיבת דואר משותפת וכו') וקיבלת את השגיאה "כתובת ה- Proxy "SMTP:alias@domain.com" כבר נמצאת בשימוש...", כתובת הדואר האלקטרוני שבחרת כבר נלקחת על-ידי אובייקט מותפשר דואר אלקטרוני אחר בארגון שלך.
  
עליך למצוא את המשתמש, הקבוצה, תיבת הדואר המשותפת או התיקיה הציבורית הכוללת כתובת דואר אלקטרוני זו ולמחוק אותה או לשנות את כתובת הדואר האלקטרוני שלה. לאחר מכן, תוכל ליצור אובייקט חדש המותפשר בדואר אלקטרוני באמצעות כתובת הדואר האלקטרוני המותפנה. השתמש בחיפוש בדף הבית כדי למצוא אותו. באפשרותך גם להשתמש בפקודה Exchange Online PowerShell הבאה כדי לחפש אותה:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
אם אינך מעוניין למחוק את כתובת הדואר האלקטרוני הקיימת, בחר כתובת דואר אלקטרוני חדשה עבור האובייקט החדש שאתה יוצר.
  