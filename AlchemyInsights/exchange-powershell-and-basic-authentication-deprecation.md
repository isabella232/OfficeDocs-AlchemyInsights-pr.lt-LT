---
title: „Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813480"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="f5e70-102">„Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas</span><span class="sxs-lookup"><span data-stu-id="f5e70-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="f5e70-103">Naujausios informacijos apie tai, kaip prisijungti prie „Exchange Online PowerShell“ nenaudojant bazinio autentifikavimo, [eikite čia](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="f5e70-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="f5e70-104">„PowerShell V2“ modulis nenaudoja bazinio autentifikavimo.</span><span class="sxs-lookup"><span data-stu-id="f5e70-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="f5e70-105">Atkreipkite dėmesį, kad Pagrindinis autentifikavimas vis dar turi būti įgalintas jūsų kliento kompiuteryje.</span><span class="sxs-lookup"><span data-stu-id="f5e70-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="f5e70-106">Naujasis „PowerShell v2“ modulis naudoja modernią autentifikavimo funkciją, kad būtų galima įjungti visas REST pagrįstas „V2 Cmdlet“ dalis.</span><span class="sxs-lookup"><span data-stu-id="f5e70-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="f5e70-107">Be „V2 Cmdlet“, taip pat suteikia galimybę pasiekti senesnes nuotolinės „PowerShell“ (RPS) „Cmdlet“, kurioms nustatyti reikalingas nuotolinis „PowerShell“ seansas.</span><span class="sxs-lookup"><span data-stu-id="f5e70-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="f5e70-108">„Windows“ kompiuteryje kuriant RPS seansą reikia, kad „WinRM BasicAuth“ būtų įgalintas kliento kompiuteryje, nors modulis naudoja modernią autentifikavimo mechanizmą, kad autentifikuotų tarnybą.</span><span class="sxs-lookup"><span data-stu-id="f5e70-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="f5e70-109">„WinRM Basic Auth“ srautas naudojamas šiuolaikiniams autentifikavimo žetonams perduoti.</span><span class="sxs-lookup"><span data-stu-id="f5e70-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="f5e70-110">Jei „WinRM Basic Auth“ išjungtas kliento kompiuteryje, nauja „V2 cmdlet“ ir toliau veiks (bet senesnė „RPS cmdlet“ – ne).</span><span class="sxs-lookup"><span data-stu-id="f5e70-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
