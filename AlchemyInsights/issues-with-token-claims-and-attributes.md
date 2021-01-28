---
title: בעיות בטענות ובתכונות של אסימונים
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035892"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="1b001-102">בעיות בטענות ובתכונות של אסימונים</span><span class="sxs-lookup"><span data-stu-id="1b001-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="1b001-103">**עדכון, קביעת תצורה או הסרה של טענות אסימון**</span><span class="sxs-lookup"><span data-stu-id="1b001-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="1b001-104">באמצעות תכלת Active Directory (תכלת לספירה), באפשרותך [להתאים אישית את סוג התביעה עבור דרישת התפקיד](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) באסימון התגובה שאתה מקבל לאחר הרשאה ליישום.</span><span class="sxs-lookup"><span data-stu-id="1b001-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="1b001-105">מפתחי יישומים יכולים להשתמש בתביעות אופציונליות ביישומי הפרסום התכולים שלהם כדי לציין אילו טענות הם מעוניינים באסימונים שנשלחו ליישום שלהם.</span><span class="sxs-lookup"><span data-stu-id="1b001-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="1b001-106">לקבלת מידע נוסף, ראה [מתן טענות אופציונליות ליישום שלך](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="1b001-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="1b001-107">[קביעת התצורה של טענות קבוצתיות עבור יישומים עם תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="1b001-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="1b001-108">אם אתה משתמש בכניסה חלקה ביישום שלך, ראה [התאמה אישית של טענות שהונפקו באסימון SAML עבור יישומים ארגוניים](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="1b001-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="1b001-109">**מיפוי תכונה של תביעות**</span><span class="sxs-lookup"><span data-stu-id="1b001-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="1b001-110">כדי לקבוע את תצורת מדיניות מיפוי התביעות באמצעות PowerShell, ראה [התאמה אישית של טענות הנפלטים באסימונים עבור יישום ספציפי בדייר (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="1b001-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="1b001-111">תכונות הרחבה של סכימת מדריך הכתובות מספקות דרך לאחסון נתונים נוספים ב-תכלת Active Directory באובייקטי משתמשים ואובייקטי מדריכי כתובות אחרים, כגון קבוצות, פרטי דייר, מנהלי שירות.</span><span class="sxs-lookup"><span data-stu-id="1b001-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="1b001-112">ניתן להשתמש רק בתכונות הרחבה באובייקטי משתמשים לצורך פליטת טענות ליישומים.</span><span class="sxs-lookup"><span data-stu-id="1b001-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="1b001-113">[שימוש בתכונות הרחבה של סכימת מדריך הכתובות בתביעות מתאר](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) כיצד להשתמש בתכונות הרחבה של סכימת directory לשליחת נתוני משתמש ליישומים בתביעות אסימונים.</span><span class="sxs-lookup"><span data-stu-id="1b001-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="1b001-114">לקבלת מידע נוסף אודות טענות token, ראה:</span><span class="sxs-lookup"><span data-stu-id="1b001-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="1b001-115">טענות באסימונים של access</span><span class="sxs-lookup"><span data-stu-id="1b001-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="1b001-116">טענות בid_token</span><span class="sxs-lookup"><span data-stu-id="1b001-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="1b001-117">[טענות](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) שניתן לצפות באסימוני מזהה ובאסימונים של access שהונפקו על-ידי תכלת AD B2C</span><span class="sxs-lookup"><span data-stu-id="1b001-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="1b001-118">הפניה לטענות של אסימון SAML</span><span class="sxs-lookup"><span data-stu-id="1b001-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
