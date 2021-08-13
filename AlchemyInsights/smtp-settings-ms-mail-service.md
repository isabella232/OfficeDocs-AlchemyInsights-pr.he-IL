---
title: הגדרות SMTP עבור Microsoft 365 הדואר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813972"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>הגדרות SMTP עבור Microsoft 365 הדואר

אלה הן הגדרות ה- SMTP עבור Microsoft 365 הדואר האלקטרוני:

**שרת**: smtp.office365.com </br>
**יציאה**: 587 </br>
**הצפנה**: STARTTLS (רק גירסת TLS 1.2 נתמכת כעת. ודא שהיישום או המכשיר שלך תומכים ב- TLS 1.2) </br>
**שם** משתמש : Office 365 שלך (לדוגמה, example@yourdomain.com) </br>
**סיסמה**: סיסמת Office 365 שלך </br>
**אימות**: נדרש </br>
**שליחת מגבלות**: 10,000 הודעות דואר אלקטרוני ביום </br>

עבור הגדרות POP ו- IMAP, ראה [הגדרות POP , IMAP ו- SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
כדי ללמוד אודות האפשרויות שלך להעביר דואר אלקטרוני באמצעות Microsoft 365 והשלבים, ראה כיצד להגדיר מכשיר או יישום רב-תכליתיים כדי לשלוח דואר אלקטרוני [באמצעות Microsoft 365 או Office 365.](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)