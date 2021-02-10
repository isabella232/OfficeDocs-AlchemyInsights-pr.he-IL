---
title: סינכרון hash של סיסמאות עבור שירות תחום
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177490"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="bde59-102">סינכרון hash של סיסמאות עבור שירות תחום</span><span class="sxs-lookup"><span data-stu-id="bde59-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="bde59-103">**אם המופע של ' תכלת AD DS ' מציג בקשה להפיכת סינכרון hash של סיסמאות לזמין**</span><span class="sxs-lookup"><span data-stu-id="bde59-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="bde59-104">אתה נתקל בתרחיש שבו אתה מפעיל סביבה היברידית שבה משתמשים מתנגדים מסביבה מקומית של תכלת Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="bde59-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="bde59-105">תרחיש זה מתקיים למרות שאתה נתקל בסינכרון hash של סיסמאות מתוך AD DS המקומי לדייר המודע של תכלת.</span><span class="sxs-lookup"><span data-stu-id="bde59-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="bde59-106">**גורם**</span><span class="sxs-lookup"><span data-stu-id="bde59-106">**Cause**</span></span>

<span data-ttu-id="bde59-107">פעולה זו מתבצעת מכיוון ש-תכלת AD Connect כברירת מחדל אינו מסנכרן רכיבי hash של מנהל LAN חדש מדור קודם (NTLM) ו-Kerberos הדרושים עבור ' תכלת AD DS '.</span><span class="sxs-lookup"><span data-stu-id="bde59-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="bde59-108">**פתרון**</span><span class="sxs-lookup"><span data-stu-id="bde59-108">**Workaround**</span></span> 

<span data-ttu-id="bde59-109">יהיה עליך לקבוע את התצורה של התחברות מסוג תכלת AD כדי לסנכרן קודי hash אלה הדרושים עבור אימות NTLM ו-Kerberos.</span><span class="sxs-lookup"><span data-stu-id="bde59-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="bde59-110">לאחר קביעת התצורה של התחברות מודעות מיידיות, האירוע ' יצירת חשבון מקומי ' או ' שינוי סיסמה ' מסנכרן גם את קודי ה-hash של הסיסמה המורשית לכיוון תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="bde59-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="bde59-111">ראה [כאן](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) לקבלת מידע נוסף על כך ולקבלת הנחיות להפיכת סינכרון סיסמאות לזמין בסביבות היברידית של תכלת AD DS.</span><span class="sxs-lookup"><span data-stu-id="bde59-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>