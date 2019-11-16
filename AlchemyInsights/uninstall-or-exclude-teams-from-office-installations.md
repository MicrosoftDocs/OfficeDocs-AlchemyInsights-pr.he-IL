---
title: הסרת התקנה או אי-הכללה של צוותים מהתקנות Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: c6d5c0233acb8fb71127dcb54c719b71aa1a5bcb
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769808"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="00d27-102">הסרה או אי-הכללה של צוותים מהתקנות חדשות או קיימות</span><span class="sxs-lookup"><span data-stu-id="00d27-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="00d27-103">צוותי Microsoft נכללים במסגרת Office 365 ProPlus, Office 365 Business ו-Office for Mac.</span><span class="sxs-lookup"><span data-stu-id="00d27-103">Microsoft Teams is included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="00d27-104">השתמש [בכלי הפריסה של office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) כדי לא לכלול צוותים מהתקנות חדשות של Office.</span><span class="sxs-lookup"><span data-stu-id="00d27-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="00d27-105">כדי *להסיר את ההתקנה* של צוותים מהתקן שבו פועל Windows, ראה [הסרת התקנה של צוותי Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="00d27-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="00d27-106">כדי לנקות צוותים של Microsoft ממחשבי יעד מרובים או ממשתמשים, ראה [שפריסת צוותי microsoft נקיה](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="00d27-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="00d27-107">השתמש באפשרות [פרומנטצוות](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) למנוע התקנה אוטומטית של צוותי Microsoft באמצעות Office.</span><span class="sxs-lookup"><span data-stu-id="00d27-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="00d27-108">השתמש באפשרות ' [התקן](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) שימוש לפני ההתקנה ', *לפני התקנת הצוותים*, כדי למנוע הפעלה אוטומטית של צוותי Microsoft לאחר ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="00d27-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="00d27-109">אם אתה משתמש ב-Office for Mac, ראה [התקנות Microsoft נבחרות ב-Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="00d27-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>