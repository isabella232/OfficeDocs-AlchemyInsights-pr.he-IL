---
title: פתרון בעיות של כניסה יחידה (SSO) חלקה עבור מקומי
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816209"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="a2e2b-102">פתרון בעיות של כניסה יחידה (SSO) חלקה עבור מקומי</span><span class="sxs-lookup"><span data-stu-id="a2e2b-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="a2e2b-103">כדי לפתור בעיות של כניסה יחידה (SSO) חלקה, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="a2e2b-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="a2e2b-104">**כיצד ניתן להתהפך על מקש הפענוח של Kerberos של חשבון המחשב של AZUREADSSO?**</span><span class="sxs-lookup"><span data-stu-id="a2e2b-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="a2e2b-105">אנו ממליצים מאוד להתגלגל מעל מקש הפענוח של Kerberos לפחות כל 30 יום.</span><span class="sxs-lookup"><span data-stu-id="a2e2b-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="a2e2b-106">כדי לבצע פעולה זו באופן ידני, ראה [כיצד להתגלגל מעל מקשי הפענוח של Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="a2e2b-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="a2e2b-107">**קביעת תצורה של SSO חלק**</span><span class="sxs-lookup"><span data-stu-id="a2e2b-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="a2e2b-108">כדי לפרוס את ה-SSO החלקה, בצע את השלבים [בכניסה היחידה של תכלת Active Directory כניסה יחידה: תחלה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="a2e2b-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="a2e2b-109">**יידוע**</span><span class="sxs-lookup"><span data-stu-id="a2e2b-109">**Advisory**</span></span>

- <span data-ttu-id="a2e2b-110">[כניסה יחידה של מדריך כניסה יחידה של Active Directory: שאלות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) נפוצות-במאמר זה, אנו מטפלים בשאלות נפוצות בנושא תכלת Active Directory חלקה אחת Sign-On (SSO חלק).</span><span class="sxs-lookup"><span data-stu-id="a2e2b-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="a2e2b-111">המשך לבדוק את התוכן החדש.</span><span class="sxs-lookup"><span data-stu-id="a2e2b-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="a2e2b-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) -מאמר זה מספק מידע לגבי האופן שבו ניתן לבצע בקשות לתכונות או לשאול שאלות טכניות אודות SSO חלק.</span><span class="sxs-lookup"><span data-stu-id="a2e2b-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="a2e2b-113">**פתרון בעיות**</span><span class="sxs-lookup"><span data-stu-id="a2e2b-113">**Troubleshoot**</span></span>

<span data-ttu-id="a2e2b-114">[פתרון בעיות של כניסה יחידה של ' תכלת Active Directory '-מאמר](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) זה עוזר לך למצוא מידע אודות פתרון בעיות בנוגע לבעיות נפוצות בנוגע לבעיות נפוצות בנושא ' תכלת Active Directory (תכלת לספירה) חלקה אחת Sign-On (SSO חלק).</span><span class="sxs-lookup"><span data-stu-id="a2e2b-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







