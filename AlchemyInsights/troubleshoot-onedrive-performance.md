---
title: פתרון ביצועים של כונן OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822199"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="ace40-102">פתרון ביצועים של כונן OneDrive</span><span class="sxs-lookup"><span data-stu-id="ace40-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="ace40-103">אם אתה נתקל בסינכרון איטי מהצפוי או בבעיות דומות בביצועים עם OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ace40-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="ace40-104">אשר שאין בעיות ידועות באמצעות [לוח המחוונים לתקינות השירות](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ace40-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="ace40-105">הפעל את ' [קבצים לפי דרישה](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) ' כך שתוכל לגשת לכל הקבצים שלך ב-onedrive מבלי להוריד את כולם ולהשתמש בשטח אחסון במכשיר.</span><span class="sxs-lookup"><span data-stu-id="ace40-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="ace40-106">[סקור את שיטות העבודה המומלצות](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) עבור תכנון וביצועים ברשת.</span><span class="sxs-lookup"><span data-stu-id="ace40-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="ace40-107">[מקסם את מהירות ההעלאה וההורדה](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), במיוחד אם אתה מסנכרן מכשיר בפעם הראשונה.</span><span class="sxs-lookup"><span data-stu-id="ace40-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="ace40-108">אם אתה מסנכרן ספריה עם יותר מ-100,000 פריטים, סינכרון OneDrive עשוי להיראות תקוע למשך זמן רב, או שהמצב מציג עיבוד 0KB של xMB. "</span><span class="sxs-lookup"><span data-stu-id="ace40-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="ace40-109">[למד עוד אודות סינכרון של יותר מ-100,000 קבצים](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , כמו גם [המגבלה הנתמכת של onedrive של קבצי 300,000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="ace40-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="ace40-110">כאשר משתמש חורג ממגבלות השימוש, SharePoint Online מוסיף בקשות נוספות מחשבון משתמש זה לתקופה קצרה.</span><span class="sxs-lookup"><span data-stu-id="ace40-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="ace40-111">כל פעולות המשתמש מנחנקו כאשר המצערת בתוקף.</span><span class="sxs-lookup"><span data-stu-id="ace40-111">All user actions are throttled while the throttle is in effect.</span></span>
