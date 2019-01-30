---
title: כלל DLP עבור ארה ב / אנגליה מספר דרכון לא עובד
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472416"
---
<span data-ttu-id="675bd-p101">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** לא עובד המכיל תוכן **ארה ב / מספר דרכון בבריטניה** בעת שימוש בסוג מידע רגיש DLP ב- O365? אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור מה המדיניות DLP הוא מחפש כאשר חישובו.</span><span class="sxs-lookup"><span data-stu-id="675bd-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="675bd-104">לדוגמה, עבור **ארה ב / מספר דרכון בבריטניה** מוגדרת עם רמת הביטחון של 75%, הבאות מוערכים והמדיניות אפשרות לזהות עבור כלל להנעת</span><span class="sxs-lookup"><span data-stu-id="675bd-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="675bd-105">**[תבנית:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** תשע ספרות</span><span class="sxs-lookup"><span data-stu-id="675bd-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="675bd-106">**[תבנית:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** תשע ספרות עוקבים</span><span class="sxs-lookup"><span data-stu-id="675bd-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="675bd-107">**[בדיקת סיכום:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** לא, קיימת ללא בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="675bd-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="675bd-108">**[הגדרה:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** מדיניות DLP הוא 75% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="675bd-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="675bd-109">הפונקציה Func_usa_uk_passport מחפש תוכן התואם את התבנית.</span><span class="sxs-lookup"><span data-stu-id="675bd-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="675bd-110">נמצאה מילת מפתח מתוך Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="675bd-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="675bd-111">לדוגמה, להפעיל דוגמת הבאה עבור **ארה ב / מספר דרכון בבריטניה** מדיניות: מספר דרכון אמריקאי 123456789</span><span class="sxs-lookup"><span data-stu-id="675bd-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="675bd-112">לקבלת מידע נוסף אודות מה נדרש עבור ארה ב / אנגליה מספר דרכון לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מראה מה ה רגיש סוגי מידע עבור ארצות הברית / מספר דרכון בבריטניה](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="675bd-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="675bd-113">באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="675bd-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
