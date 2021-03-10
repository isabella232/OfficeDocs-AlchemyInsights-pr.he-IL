---
title: פתרון בעיות באישורי חתימה של SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693422"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="d47c1-102">פתרון בעיות באישורי חתימה של SAML</span><span class="sxs-lookup"><span data-stu-id="d47c1-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="d47c1-103">כדי לפתור את בעיית אישור החתימה של SAML, בצע את השלבים המומלצים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d47c1-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="d47c1-104">בעת הוספת יישום ארגוני התומך ב-SSO, התכלת יפיק אישור שנקרא ' [אישור חתימה של SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)'.</span><span class="sxs-lookup"><span data-stu-id="d47c1-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="d47c1-105">אישור זה מכיל תאריך תפוגה של 3 שנים.</span><span class="sxs-lookup"><span data-stu-id="d47c1-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="d47c1-106">כדי לשנות את תאריך התפוגה של האישור, ראה [התאמה אישית של תאריך התפוגה של אישור האיחוד והעברתה לאישור חדש](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="d47c1-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="d47c1-107">האפשרות ' תכלת ' תשתמש באישור זה כדי להחתים את האסימונים של SAML המבוקשים על-ידי היישום ולשלוח אותו ליישום עבור SSO מוצלח.</span><span class="sxs-lookup"><span data-stu-id="d47c1-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="d47c1-108">כדי להשלים זאת, הורד את האישור מפורטל התכלת ושלח אותו לספק היישומים כדי להשלים את תהליך ה-SSO.</span><span class="sxs-lookup"><span data-stu-id="d47c1-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="d47c1-109">לאחר השלמת תהליך זה, היישום יאפשר לך לתת אמון באישור זה וכל האסימונים של SAML שנחתמו על-ידי אישור זה יתקבלו על-ידי היישום.</span><span class="sxs-lookup"><span data-stu-id="d47c1-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="d47c1-110">אם תוקף אישור זה פג, צור אישור חדש, עדכן אותו לספק היישומים ולאחר מכן הפוך אותו לפעיל בצד התכלת.</span><span class="sxs-lookup"><span data-stu-id="d47c1-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="d47c1-111">לקבלת מידע נוסף, ראה [חידוש אישור שיפוג בקרוב](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="d47c1-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="d47c1-112">אם פג תוקפו של האישור, המשתמש לא נחסם.</span><span class="sxs-lookup"><span data-stu-id="d47c1-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="d47c1-113">[הוסף כתובת דואר אלקטרוני לקבלת הודעות](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) שיתקבלו לפני שפג תוקפו של האישור הנוכחי.</span><span class="sxs-lookup"><span data-stu-id="d47c1-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="d47c1-114">שלב 4 הוא אופציונלי.</span><span class="sxs-lookup"><span data-stu-id="d47c1-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="d47c1-115">שינוי אפשרויות חתימת האישורים של SAML והאלגוריתם לחתימת אישור.</span><span class="sxs-lookup"><span data-stu-id="d47c1-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="d47c1-116">לקבלת מידע נוסף, ראה [שינוי אפשרויות חתימת אישורים והוספת אלגוריתם חתימה](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="d47c1-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

