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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717570"
---
# <a name="fix-dkim-setup-issues"></a>DKIM sąrankos problemų sprendimas

Jei kyla problemų įgalinant DKIM savo pasirinktinį domeną, atlikite šiuos veiksmus:

- Dauguma DKIM sąrankos problemos yra susijusios su neteisingudns įrašus. Patikrinkite, ar DKIM CNAME įrašas **(ne** TXT įrašas) yra tinkamai suformatuotas. Daugiau informacijos ieškokite šioje [temoje](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Sukūrę arba atnaujinę savo DKIM DNS įrašus domeno DNS išteklių nuomos tarnyboje (paprastai domenų registratoriuje), palaukite, kol DNS įrašai bus platinami.

- Jei negalite sukurti DKIM DNS įrašų administravimo centre, \<galite\> pakeisti CustomDomain savo pasirinktinį domeną (pvz., `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`contoso.com) ir paleisti šią komandą ["Exchange Online PowerShell":](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).
