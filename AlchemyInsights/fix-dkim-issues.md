---
title: DKIM sąrankos problemų sprendimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765241"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="57f57-102">DKIM sąrankos problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="57f57-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="57f57-103">Jei kyla nesklandumų, leidžianti DKIM pasirinktinio domeno, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="57f57-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="57f57-104">Dauguma DKIM nustatymo problemos yra susijusios su neteisingas DNS įra us.</span><span class="sxs-lookup"><span data-stu-id="57f57-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="57f57-105">Patikrinkite, ar teisingai suformatuotas DKIM CNAME įrašą (**ne** TXT įrašą).</span><span class="sxs-lookup"><span data-stu-id="57f57-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="57f57-106">Norėdami gauti daugiau informacijos, peržiūrėkite šią [temą](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="57f57-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="57f57-107">Po to, kai sukurti arba atnaujinti savo DKIM DNS įra us DNS išteklių nuomos tarnybos domeno (paprastai domenų registratoriaus), palaukti, kol DNS įrašai platinti.</span><span class="sxs-lookup"><span data-stu-id="57f57-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="57f57-108">Jei jūs negalite sukurti DKIM DNS įrašų administravimo centro, jūs galite pakeisti \<CustomDomain\> su savo individualiame domene (pvz.,.: contoso.com) ir vykdykite šią komandą į [Exchange Online "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="57f57-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
