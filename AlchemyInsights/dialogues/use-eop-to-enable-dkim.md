---
title: שימוש ב-Exchange Online PowerShell כדי להפוך את DKIM לזמין עבור תחום ספציפי
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524175"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="e40fc-102">שימוש ב-Exchange Online PowerShell כדי להפוך את DKIM לזמין עבור תחום ספציפי</span><span class="sxs-lookup"><span data-stu-id="e40fc-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="e40fc-103">אם אין באפשרותך ליצור את רשומות ה-DNS של DKIM במרכז הניהול, נסה להשתמש ב-Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e40fc-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="e40fc-104">כדי ליצור רשומת DNS של DKIM באמצעות Exchange Online PowerShell, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e40fc-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="e40fc-105">פתח את Windows PowerShell כמנהל מערכת והפעלת הפקודות הבאות ברצף המתואר:</span><span class="sxs-lookup"><span data-stu-id="e40fc-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="e40fc-106">מ.</span><span class="sxs-lookup"><span data-stu-id="e40fc-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="e40fc-107">b.</span><span class="sxs-lookup"><span data-stu-id="e40fc-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="e40fc-108">c.</span><span class="sxs-lookup"><span data-stu-id="e40fc-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="e40fc-109">אם אתה נתקל בבעיות בהתחברות ל-Exchange Online PowerShell, ראה [התחברות אל Exchange Online powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="e40fc-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="e40fc-110">לאחר שאתה מחובר ל-Exchange Online PowerShell, הפעלת הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="e40fc-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="e40fc-111">לאחר שהפקודה לעיל בוצעה בהצלחה, הפעל את הפקודה הבאה כדי לסיים את ההפעלה של Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e40fc-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 


