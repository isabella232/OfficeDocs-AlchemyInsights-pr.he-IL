---
title: תצורה וירטואלית באמצעות שירותי תחומים של ה-עמ
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
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885203"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>תצורה וירטואלית באמצעות שירותי תחומים של ה-עמ

התצורה הווירטואלית עם שירותי התחום של ה-עמ מערבת את השלבים 

1. בדיקת תקינות התחום שלך בפורטל התכלת https://aka.ms/aadds-health
2. בדיקת הNSG עבור כללים החוסמים את היציאות הדרושות כדי לסנכרן בשירותי התחומים של תכלת AD בפורטל https://aka.ms/aadds-networking
3. להבטיח שהרשת הוירטואלית שלך נפרסת באותו אזור תכלת כתחום המנוהל על-ידי תכלת AD Domain.
4. להבטיח שאין לך תחום קיים עם אותו שם תחום זמין ברשת הוירטואלית.

לקבלת פרטים נוספים על התחשבות בעיצוב ברשת הווירטואלית של תכלת כדי לתמוך בשירותי תחום של ה-עמ, ראה [שיקול הרשת הוירטואלי](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

