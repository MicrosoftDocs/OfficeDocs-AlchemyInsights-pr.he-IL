---
title: 902 (שגיאות סינכרון עקב אובייקטים כפולים)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472807"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="06d7b-102">שגיאות סינכרון עקב שכפול עצמים</span><span class="sxs-lookup"><span data-stu-id="06d7b-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="06d7b-103">ייתכן שתקבל אחת מהודעות השגיאה הבאות בעת סיום סינכרון ספריות:</span><span class="sxs-lookup"><span data-stu-id="06d7b-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="06d7b-104">אין אפשרות לעדכן אובייקט זה ב- Microsoft Online Services מכיוון התכונות הבאות המשויך לאובייקט זה יש ערכים שייתכן כבר משוייכים לאובייקט אחר בספריה המקומית שלך.</span><span class="sxs-lookup"><span data-stu-id="06d7b-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="06d7b-105">אובייקט מסונכרן עם אותה כתובת proxy כבר קיים בספריה שלך השירותים המקוונים של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="06d7b-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="06d7b-106">אין אפשרות לעדכן אובייקט זה מכיוון התכונות הבאות המשויך לאובייקט זה יש ערכים שייתכן כבר משוייכים לאובייקט אחר בשירותי הספריות המקומי שלך: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="06d7b-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="06d7b-107">כדי לזהות ולתקן את הבעיה, להוריד ולהפעיל את [הכלי תיקון שגיאה של DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="06d7b-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="06d7b-108">לקבלת מידע נוסף, ראה [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="06d7b-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  
