---
title: „Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015697"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="46ac2-102">„Exchange PowerShell“ ir bazinio autentifikavimo atsisakymas</span><span class="sxs-lookup"><span data-stu-id="46ac2-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="46ac2-103">Naujausios informacijos apie tai, kaip prisijungti prie „Exchange Online PowerShell“ nenaudojant bazinio autentifikavimo, [eikite čia](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="46ac2-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="46ac2-104">Atkreipkite dėmesį, kad Pagrindinis autentifikavimas vis dar turi būti įgalintas jūsų kliento kompiuteryje.</span><span class="sxs-lookup"><span data-stu-id="46ac2-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="46ac2-105">Naujasis „PowerShell v2“ modulis naudoja modernią autentifikavimo funkciją, kad būtų galima įjungti visas REST pagrįstas „V2 Cmdlet“ dalis.</span><span class="sxs-lookup"><span data-stu-id="46ac2-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="46ac2-106">Be „V2 Cmdlet“, taip pat suteikia galimybę pasiekti senesnes nuotolinės „PowerShell“ (RPS) „Cmdlet“, kurioms nustatyti reikalingas nuotolinis „PowerShell“ seansas.</span><span class="sxs-lookup"><span data-stu-id="46ac2-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="46ac2-107">„Windows“ kompiuteryje kuriant RPS seansą reikia, kad „WinRM BasicAuth“ būtų įgalintas kliento kompiuteryje, nors modulis naudoja modernią autentifikavimo mechanizmą, kad autentifikuotų tarnybą.</span><span class="sxs-lookup"><span data-stu-id="46ac2-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="46ac2-108">„WinRM Basic Auth“ srautas naudojamas šiuolaikiniams autentifikavimo žetonams perduoti.</span><span class="sxs-lookup"><span data-stu-id="46ac2-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="46ac2-109">Jei „WinRM Basic Auth“ išjungtas kliento kompiuteryje, nauja „V2 cmdlet“ ir toliau veiks (bet senesnė „RPS cmdlet“ – ne).</span><span class="sxs-lookup"><span data-stu-id="46ac2-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
