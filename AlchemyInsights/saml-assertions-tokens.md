---
title: הצהרת SAML (אסימונים)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885215"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="cbfc1-102">הצהרת SAML (אסימונים)</span><span class="sxs-lookup"><span data-stu-id="cbfc1-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="cbfc1-103">האסימונים של ' הצהרות אבטחה ' (SAML) הם ייצוגי XML של טענות.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="cbfc1-104">כברירת מחדל, משתמשים ב-SAML tokens של יסודות התקשורת של Windows (WCF) בתרחישים של אבטחה מאוחדת מונפקים אסימונים.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="cbfc1-105">לקבלת מידע נוסף, ראה [אסימונים וטענות של SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="cbfc1-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="cbfc1-106">פלטפורמת הזהויות של Microsoft פולטת כמה סוגים של אסימוני אבטחה בעיבוד של כל זרימת אימות.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="cbfc1-107">[הפניה לטענות אסימון SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) מתארת את העיצוב, מאפייני האבטחה והתוכן של SAML 2.0.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="cbfc1-108">פעל לפי ההנחיות [באורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) כדי להבין כיצד לקבוע אורך חיים של אסימונים.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="cbfc1-109">בצע את השלבים המתוארים [במאמר זה](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) כדי להבין כיצד לקבוע את התצורה של הצפנת אסימון מסוג תכלת AD SAML.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="cbfc1-110">ב-תכלת לספירה, באפשרותך להגדיר אפשרויות חתימת אישורים ואת אלגוריתם חתימת האישורים.</span><span class="sxs-lookup"><span data-stu-id="cbfc1-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="cbfc1-111">לקבלת מידע נוסף, ראה [אפשרויות של חתימת אישורים מתקדמת באסימון SAML עבור יישומי גלריה ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="cbfc1-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
