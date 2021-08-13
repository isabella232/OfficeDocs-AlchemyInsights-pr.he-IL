---
title: מגבלות עבור תוויות רגישות עבור Office קבצים SharePoint וקבצים OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813156"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>מגבלות עבור תוויות רגישות עבור Office קבצים SharePoint וקבצים OneDrive

בעת הפיכת תוויות רגישות לזמינים עבור Office קבצים ב- SharePoint ו- OneDrive, שים לב לדרישות ולמגבלות, הכוללות:

- SharePoint ו- OneDrive אין אפשרות לעבד קבצים מסוימים עם תוויות ומוצפנים מאפליקציות שולחן העבודה של Office כאשר הקבצים מכילים נתוני PowerQuery, נתונים המאוחסנים על-ידי תוספות מותאמות אישית או חלקי XML מותאמים אישית.
- SharePoint ו OneDrive אל תחיל תוויות רגישות באופן אוטומטי על קבצים קיימים שכבר הצפנת באמצעות תוויות Azure Information Protection (AIP). כדי להחיל תוויות רגישות על קבצים מוצפנים: 
    - ודא שתוויות AIP הועברו ופורסמו במרכז Microsoft 365 תאימות.
    - הורד את הקבצים עם התווית ולאחר מכן העלה אותם למיקום SharePoint או OneDrive שלהם.
- עבור מסמכים מוצפנים, הדפסה אינה נתמכת.

לקבלת פרטים נוספים על מגבלות, ראה הפיכת תוויות רגישות [לזמינות עבור Office קבצים SharePoint וקבצים OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
