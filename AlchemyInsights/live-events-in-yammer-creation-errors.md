---
title: שגיאות יצירה של אירועים בשידור חי ב- Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947889"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="bbfef-102">שגיאות יצירה של אירועים בשידור חי ב- Yammer</span><span class="sxs-lookup"><span data-stu-id="bbfef-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="bbfef-103">**יצירת אירועים בשידור חי של Yammer**</span><span class="sxs-lookup"><span data-stu-id="bbfef-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="bbfef-104">Yammer יציג את האפשרות ליצור אירוע חי בכל עת.</span><span class="sxs-lookup"><span data-stu-id="bbfef-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="bbfef-105">במקרים מסוימים, ייתכן שמשתמש לא יעמוד בדרישות המוקדמות ליצירת אירוע חי ויקבל הודעת שגיאה כאשר הוא ינסה ליצור אותו.</span><span class="sxs-lookup"><span data-stu-id="bbfef-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="bbfef-106">הפריטים שלהלן מכסים את הסיבות הנפוצות לבעיה זו ומספקים דרכים לפתרון הבעיה עבור משתמשי הקצה.</span><span class="sxs-lookup"><span data-stu-id="bbfef-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="bbfef-107">**מי יכול ליצור אירועים בשידור חי**</span><span class="sxs-lookup"><span data-stu-id="bbfef-107">**Who can create live events**</span></span>
- <span data-ttu-id="bbfef-108">רישיון Office 365 Enterprise E1, E3, או E5 או רישיון Office 365 A3 או רישיון A5.</span><span class="sxs-lookup"><span data-stu-id="bbfef-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="bbfef-109">הרשאה ליצירת אירועים בשידור חי במרכז הניהול של Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bbfef-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="bbfef-110">הרשאה ליצירת אירועים בשידור חי ב- Microsoft Stream (עבור אירועים שמופקים באמצעות יישום או מכשיר שידור חיצוני).</span><span class="sxs-lookup"><span data-stu-id="bbfef-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="bbfef-111">חברות צוות מלאה בארגון (אינך יכול להיות אורח או מארגון אחר)</span><span class="sxs-lookup"><span data-stu-id="bbfef-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="bbfef-112">האפשרויות קביעת מועד פגישה פרטית, שיתוף מסך ושיתוף IP וידאו צריכות להיות מופעלות במדיניות פגישת צוות.</span><span class="sxs-lookup"><span data-stu-id="bbfef-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="bbfef-113">**מדיניות יצירת אירוע בשידור חי**</span><span class="sxs-lookup"><span data-stu-id="bbfef-113">**Live event creation policies**</span></span>

<span data-ttu-id="bbfef-114">Yammer מציית לפריטי מדיניות אירוע בשידור חי אשר הוגדרו בדיירOffice 365 עבור Stream.</span><span class="sxs-lookup"><span data-stu-id="bbfef-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="bbfef-115">כברירת מחדל, כל המשתמשים בארגון יכולים ליצור אירוע בשידור חי.</span><span class="sxs-lookup"><span data-stu-id="bbfef-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="bbfef-116">מנהלי מערכת יכולים [לבצע שינויים בהגדרה זו, דבר שעשוי למנוע מהמשתמשים ליצור אירוע בשידור חי](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="bbfef-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="bbfef-117">חשוב לבדוק שלמשתמשים יש הרשאות ליצירת אירועים בשידור חי אם הם מקבלים שגיאת מדיניות.</span><span class="sxs-lookup"><span data-stu-id="bbfef-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>