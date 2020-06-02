---
title: DKIM sąrankos problemų sprendimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506782"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="a1a90-102">DKIM sąrankos problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="a1a90-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="a1a90-103">Jei kyla problemų įgalinant DKIM savo pasirinktinį domeną, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a1a90-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="a1a90-104">Dauguma DKIM sąrankos problemos yra susijusios su neteisingudns įrašus.</span><span class="sxs-lookup"><span data-stu-id="a1a90-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="a1a90-105">Patikrinkite, ar DKIM CNAME įrašas **(ne** TXT įrašas) yra tinkamai suformatuotas.</span><span class="sxs-lookup"><span data-stu-id="a1a90-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="a1a90-106">Daugiau informacijos ieškokite šioje [temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="a1a90-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="a1a90-107">Sukūrę arba atnaujinę savo DKIM DNS įrašus domeno DNS išteklių nuomos tarnyboje (paprastai domenų registratoriuje), palaukite, kol DNS įrašai bus platinami.</span><span class="sxs-lookup"><span data-stu-id="a1a90-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="a1a90-108">Jei negalite sukurti DKIM DNS įrašų administravimo centre, galite pakeisti \<CustomDomain\> savo pasirinktinį domeną (pvz., contoso.com) ir paleisti šią komandą ["Exchange Online PowerShell":](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="a1a90-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
