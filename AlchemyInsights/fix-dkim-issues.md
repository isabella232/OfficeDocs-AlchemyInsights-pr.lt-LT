---
title: "\"DKIM\" sąrankos problemų sprendimas"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744958"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="094d3-102">"DKIM" sąrankos problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="094d3-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="094d3-103">Jei susiduriate su problemomis, įgalinančiomis DKIM jūsų pasirinktiniam domenui, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="094d3-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="094d3-104">Daugelis DKIM sąrankos problemų yra susijusios su klaidingais DNS įrašais.</span><span class="sxs-lookup"><span data-stu-id="094d3-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="094d3-105">Patikrinkite, ar teisingai suformatuotas DKIM CNAME įrašas (**ne** txt įrašas).</span><span class="sxs-lookup"><span data-stu-id="094d3-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="094d3-106">Daugiau informacijos ieškokite šioje [temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="094d3-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="094d3-107">Kai "DKIM" DNS įrašus sukuriate arba naujinate savo domeno DNS išteklių nuomos tarnyboje (paprastai jūsų domenų registratorius), palaukite, kol DNS įrašus išplatins.</span><span class="sxs-lookup"><span data-stu-id="094d3-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="094d3-108">Jei negalite sukurti DKIM DNS įrašus administravimo centre, galite pakeisti \<CustomDomain\> savo pasirinktinio domeno (pvz., contoso.com) ir paleisti šią komandą " [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)" "PowerShell": `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="094d3-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
