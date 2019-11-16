---
title: הגדרות מדיניות פגישה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376664"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="1a825-102">ניהול מדיניות פגישה בצוותי Microsoft</span><span class="sxs-lookup"><span data-stu-id="1a825-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="1a825-103">מדיניות פגישה משמשת לשליטה בתכונות הזמינות לפגישה עם משתתפים בפגישות שתוזמנו על-ידי משתמשים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="1a825-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="1a825-104">ייתכן שחלק מהתכונות של מדיניות הפגישה לא יושמו במרכז הניהול של הצוותים עדיין (אלה מתויגים "בקרוב" בתיעוד).</span><span class="sxs-lookup"><span data-stu-id="1a825-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="1a825-105">במקרה זה, או אם אתה מקבל שגיאה כמו "אנחנו לא יכולים לעדכן את המדיניות עכשיו, אבל לנסות את זה שוב מאוחר יותר" במרכז הניהול של צוותי Microsoft, אנו ממליצים להשתמש ב-PowerShell כדי ליצור או לשנות מדיניות פגישה של צוותים.</span><span class="sxs-lookup"><span data-stu-id="1a825-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="1a825-106">לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1a825-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="1a825-107">כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="1a825-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="1a825-108">כדי לבצע שינויי מדיניות באמצעות יישומוני cmdlet PowerShell, ראה [קבוצות מבט כולל של powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="1a825-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="1a825-109">אתה צריך להשתמש [סקייפ עבור עסקים PowerShell מודול](https://www.microsoft.com/download/details.aspx?id=39366) עבור צוותי מדיניות פגישה.</span><span class="sxs-lookup"><span data-stu-id="1a825-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="1a825-110">בדוק את [התיעוד \*-c, מדיניות יישומוני ה-cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="1a825-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="1a825-111">**הערה:** זה יכול להימשך עד 24 שעות כדי שהשינויים במדיניות ייכנסו לתוקף עבור משתמשים.</span><span class="sxs-lookup"><span data-stu-id="1a825-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="1a825-112">ייתכן שלא תוכל לבצע שינויים בפריטי מדיניות חדשים שנוצרו באופן מיידי; המתן 4 שעות ונסה לשנות שוב מדיניות חדשה שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="1a825-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="1a825-113">אם עדיין יש לך בעיות, נסה PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1a825-113">If you're still having problems, try PowerShell.</span></span>  