---
title: אין אפשרות למחוק פריטים ב- SharePoint או OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757926"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b1eb9-102">אין אפשרות למחוק פריטים</span><span class="sxs-lookup"><span data-stu-id="b1eb9-102">Unable to delete items</span></span>

<span data-ttu-id="b1eb9-103">נתקל בבעיות מחיקת פריטים?</span><span class="sxs-lookup"><span data-stu-id="b1eb9-103">Having issues deleting items?</span></span>

- <span data-ttu-id="b1eb9-104">הקפד תמיד שיש לך את [ההרשאות המתאימות](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) כדי למחוק את הפריט או להיות בעל ניסיון [מנהל אוסף אתרים](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) להסיר את הפריט.</span><span class="sxs-lookup"><span data-stu-id="b1eb9-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="b1eb9-105">ודא כי אין הגדרת [מדיניות שמירה](https://docs.microsoft.com/office365/securitycompliance/retention-policies) פריט.</span><span class="sxs-lookup"><span data-stu-id="b1eb9-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="b1eb9-106">ודא שהפריט אינו [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) אל משתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="b1eb9-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="b1eb9-107">לבסוף, מנהלי מערכת יכולים להשתמש [תבניות SharePoint ותרגולים](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) אשר מכיל ספריה של PowerShell פקודות המאפשרות לך לבצע פעולות ניהול מורכבים כגון לכפות את מחיקת פריטים stubborn.</span><span class="sxs-lookup"><span data-stu-id="b1eb9-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="b1eb9-108">הסרת קובץ PNP</span><span class="sxs-lookup"><span data-stu-id="b1eb9-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b1eb9-109">הסרת תיקיה PNP</span><span class="sxs-lookup"><span data-stu-id="b1eb9-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b1eb9-110">הסר פריט רשימה PNP</span><span class="sxs-lookup"><span data-stu-id="b1eb9-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b1eb9-111">הסר את רשימת PNP</span><span class="sxs-lookup"><span data-stu-id="b1eb9-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b1eb9-112">הסרת PNP שדה (עמודה)</span><span class="sxs-lookup"><span data-stu-id="b1eb9-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)