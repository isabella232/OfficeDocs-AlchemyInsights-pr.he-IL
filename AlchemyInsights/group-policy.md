---
title: מדיניות קבוצתית
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256777"
---
# <a name="group-policy"></a>מדיניות קבוצתית

הגדרות עבור אובייקטי משתמשים ומחשבים ב-תכלת Active Directory Domain Services (תכלת AD DS) מנוהלות לעתים קרובות באמצעות אובייקטי מדיניות קבוצתית (Gpo). תכלת AD DS כולל אובייקטי Gpo מוכללים עבור משתמשי AADDC ומיכלי AADDC של מחשבים. באפשרותך להתאים אישית אובייקטי Gpo מוכללים אלה כדי לקבוע תצורה של מדיניות קבוצתית לפי הצורך עבור הסביבה שלך. לחברים בקבוצת מנהלי המערכת של תכלת לספירה יש הרשאות של ניהול מדיניות קבוצתית בתחום תכלת AD DS, וניתן גם ליצור אובייקטי Gpo ויחידות ארגוניות מותאמות אישית (Ou). לקבלת מידע נוסף אודות המדיניות הקבוצתית ואופן הפעולה שלה, ראה [מבט כולל על מדיניות קבוצתית](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

בסביבה היברידית, פריטי מדיניות קבוצתית שתצורתם נקבעה בסביבת AD DS מקומית אינם מסונכרנים עם התכלת AD DS. כדי להגדיר הגדרות תצורה עבור משתמשים או מחשבים ב-תכלת AD DS, ערוך אחד מאובייקטי ה-Gpo המהווים ברירת מחדל או צור GPO מותאם אישית.

מאמר זה [ניהול מדיניות קבוצתית](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) מראה לך כיצד להתקין את כלי ניהול המדיניות הקבוצתית, כיצד טון לערוך את אובייקטי ה-gpo המוכללים וכיצד ליצור אובייקטי gpo מותאמים אישית.



