---
title: שינוי דרישת סיסמה חזקה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818469"
---
# <a name="change-strong-password-requirement"></a>שינוי דרישת סיסמה חזקה

Microsoft דורשת סיסמאות חזקות כברירת מחדל.

באמצעות PowerShell, באפשרותך להפוך סיסמאות חזקות ללא זמינות עבור משתמשים ספציפיים באמצעות פקודות אלה:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

כדי להפוך סיסמאות חזקות ללא זמינות עבור כל המשתמשים, השתמש ב:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [מידע נוסף אודות מדיניות סיסמאות](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [כיצד להתחבר ל- Microsoft 365 באמצעות PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [מידע נוסף אודות פקודות PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
