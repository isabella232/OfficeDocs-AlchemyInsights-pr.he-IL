---
title: רמות הרשאה של SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716893"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer בעיות חיבור 

<p>אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נא נסה את הפתרונות הבאים נפוצים.</p> <p><strong>שלב 1:</strong> <strong>לאמת SharePoint Designer מתעדכן&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer ה-Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">עדכון עבור SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>שלב 2:</strong> <strong>נקה את קבצי מטמון מקומי</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">סגור את SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">במחשב המקומי, לאתר את התיקיות הבאות כדי להסיר קבצים במטמון.&nbsp;</li> <li style="font-weight: 400;">לחץ על <strong>התחל -&gt; להפעיל</strong> ומחק את כל הקבצים שנמצאו תחת כל אחד להלן מיקומים.&nbsp;<br /><br />Extensions\Cache שרת %APPDATA%\Microsoft\Web<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">פתח את SharePoint Designer 2013 והזן את החשבון שוב כדי לראות אם הוא פועל.</li> </ol> <p><strong>שלב 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>להפעיל אימות מודרני עבור 2013 Office בהתקני Windows</strong></a>&nbsp;</p> <p><strong>שלב 4:</strong> <strong>מנהלים יהיה עליך לאפשר קובץ Script מותאם אישית כדי לאפשר את החיבור SharePoint Designer</strong>.</p> <p>לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">אפשר או מנע בקובץ script מותאם אישית</a>.&nbsp;</p>


