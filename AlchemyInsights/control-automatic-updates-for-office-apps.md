---
title: שלוט בעדכונים אוטומטיים עבור יישומי Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439332"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="4251a-102">שלוט בעדכונים אוטומטיים עבור יישומי Office</span><span class="sxs-lookup"><span data-stu-id="4251a-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="4251a-103">כברירת מחדל, עדכונים עבור יישומי Office מורדים באופן אוטומטי ומוחלים ברקע ללא התערבות של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="4251a-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="4251a-104">עם זאת, מנהלי מערכת יכולים לשלוט באופן החלת העדכונים באמצעות הגדרות Office Update.</span><span class="sxs-lookup"><span data-stu-id="4251a-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="4251a-105">הגדרות עדכון מאפשרות למנהלי מערכת להפעיל או להשבית עדכונים אוטומטיים, להציג או להסתיר את לחצן ' **עדכן כעת** ' ב-Office, לקבוע תאריכי יעד לעדכון ועוד.</span><span class="sxs-lookup"><span data-stu-id="4251a-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="4251a-106">למידע מפורט, ראו:</span><span class="sxs-lookup"><span data-stu-id="4251a-106">For detailed information, see:</span></span>

- [<span data-ttu-id="4251a-107">קביעת תצורה של הגדרות עדכון עבור Office</span><span class="sxs-lookup"><span data-stu-id="4251a-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="4251a-108">העדכון האוטומטי עבור Office אינו זמין</span><span class="sxs-lookup"><span data-stu-id="4251a-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="4251a-109">הגדרת אופן העדכון של Office לאחר התקנתו</span><span class="sxs-lookup"><span data-stu-id="4251a-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="4251a-110">כדי לסקור את הגדרות העדכונים הקיימים שהוחלו על מחשב לקוח, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="4251a-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="4251a-111">פתח את עורך הרישום על-ידי **הפעלת**  >  **הפעלת**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="4251a-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="4251a-112">עבור למיקום הבא וסקור את הגדרות Office Update:</span><span class="sxs-lookup"><span data-stu-id="4251a-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="4251a-113">קצת.</span><span class="sxs-lookup"><span data-stu-id="4251a-113">a.</span></span> <span data-ttu-id="4251a-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="4251a-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="4251a-115">b.</span><span class="sxs-lookup"><span data-stu-id="4251a-115">b.</span></span> <span data-ttu-id="4251a-116">לחץ על \ קביעת תצורה</span><span class="sxs-lookup"><span data-stu-id="4251a-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="4251a-117">**שים לב**  אם המפתח הרפואי מוגדר, ייתכן שתראה את ההודעה "העדכונים מנוהלים על-ידי מנהל המערכת **Office**"  >  **Account**  >  **בעדכונים של office**לחשבון office.</span><span class="sxs-lookup"><span data-stu-id="4251a-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="4251a-118">לקבלת מידע נוסף, ראה [ניהול עדכונים ל-Microsoft 365 Apps עם מנהל תצורת נקודות הקצה של microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="4251a-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  