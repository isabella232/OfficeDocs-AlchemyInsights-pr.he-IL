---
title: שגיאות כניסה למשתמש
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900991"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="fa3d7-102">שגיאות כניסה למשתמש</span><span class="sxs-lookup"><span data-stu-id="fa3d7-102">User sign-in errors</span></span>

<span data-ttu-id="fa3d7-103">**פתרון בעיות באבחון הכניסה**</span><span class="sxs-lookup"><span data-stu-id="fa3d7-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="fa3d7-104">כדי לזהות את הסיבה או לאבחן בעיות הקשורות לכניסה למשתמש, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="fa3d7-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="fa3d7-105">הפעל את [אבחון הכניסה](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="fa3d7-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="fa3d7-106">אתר את האירוע לניתוח על-ידי הזנת הפרטים הדרושים לך אודות המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.</span><span class="sxs-lookup"><span data-stu-id="fa3d7-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="fa3d7-107">סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואילו פעולות ניתן לבצע כדי לבצע שינויים, אם נדרשים שינויים כלשהם.</span><span class="sxs-lookup"><span data-stu-id="fa3d7-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="fa3d7-108">**מחפש מידע לגבי קודי השגיאה של AADSTS המוחזרים משירות ה-"תכלת Active Directory (תכלת לספירה) שירות אסימוני אבטחה (STS)?**</span><span class="sxs-lookup"><span data-stu-id="fa3d7-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="fa3d7-109">קרא [מאמר זה](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) כדי למצוא תיאורי שגיאות של AADSTS, תיקונים ומספר פתרונות מוצעים</span><span class="sxs-lookup"><span data-stu-id="fa3d7-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>