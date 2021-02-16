---
title: התקן Writeback
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256851"
---
# <a name="device-writeback"></a><span data-ttu-id="5364e-102">התקן Writeback</span><span class="sxs-lookup"><span data-stu-id="5364e-102">Device Writeback</span></span>

<span data-ttu-id="5364e-103">התקן Writeback נמצא בשימוש בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5364e-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="5364e-104">[הפוך את Windows שלום לזמין לעסקים באמצעות פריסת אישורים היברידית](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="5364e-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="5364e-105">הפיכת גישה מותנית לזמינה בהתבסס על מכשירים ב-ADFS (2012 R2 או גבוה יותר) יישומים מוגנים (יחסי הסתמכות של מפלגת השקר)</span><span class="sxs-lookup"><span data-stu-id="5364e-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="5364e-106">נדרש מנוי לתכלת AD Premium עבור writeback של התקן.</span><span class="sxs-lookup"><span data-stu-id="5364e-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="5364e-107">פעולה זו מספקת אבטחה נוספת והבטחה לכך שגישה ליישומים מוענקה רק למכשירים מהימנים.</span><span class="sxs-lookup"><span data-stu-id="5364e-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="5364e-108">לקבלת מידע נוסף אודות גישה מותנית, ראה [ניהול סיכונים באמצעות גישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) [והגדרת גישה מותנית מקומית באמצעות הרישום של התקן תכלת של active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="5364e-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="5364e-109">לקבלת מידע נוסף אודות הפעלת Writeback של מכשירים עבור מכשירים, ראה [הפיכת התקן לזמין Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span><span class="sxs-lookup"><span data-stu-id="5364e-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
