---
title: "\"SharePoint Online PowerShell\""
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770847"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="46a4d-102">"SharePoint Online PowerShell"</span><span class="sxs-lookup"><span data-stu-id="46a4d-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="46a4d-103">Darbas su "PowerShell" arba scenarijais naudojant "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="46a4d-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="46a4d-104">Daugiau informacijos rasite apsilankę toliau pateiktose nuorodose.</span><span class="sxs-lookup"><span data-stu-id="46a4d-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="46a4d-105">Darbo su "SharePoint Online Management Shell" Pradžia</span><span class="sxs-lookup"><span data-stu-id="46a4d-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="46a4d-106">Prisijungimas prie "SPO PowerShell" naudojant kelių dalių autentifikavimą (MFA)</span><span class="sxs-lookup"><span data-stu-id="46a4d-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="46a4d-107">" [SharePoint" trafaretai ir praktika (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) yra "PowerShell" komandų biblioteka, leidžianti atlikti sudėtingus valdymo veiksmus siekiant SPO.</span><span class="sxs-lookup"><span data-stu-id="46a4d-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="46a4d-108">Jei kyla problemų jungiantis naudojant SPO valdymo aplinką, įsitikinkite, kad atnaujinote į naujausią versiją ir bandote [iš naujo importuoti modulį](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) naudodami *"Import-Module Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="46a4d-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="46a4d-109">Jei bandote paleisti kliento pusės objekto modelio scenarijus, jums reikės " [SharePoint Online" kliento komponentų SDK](https://www.microsoft.com/download/details.aspx?id=42038) įdiegtą vietiniame kompiuteryje.</span><span class="sxs-lookup"><span data-stu-id="46a4d-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="46a4d-110">Jei kyla problemų paleidus "PowerShell" scenarijus, galbūt norėsite "PowerShell" paleisti administratoriaus teisėmis ir pakeisti [vykdymo strategiją](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="46a4d-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>