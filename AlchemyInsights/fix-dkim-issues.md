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
# <a name="fix-dkim-setup-issues"></a>DKIM sąrankos problemų sprendimas

Jei kyla problemų įgalinant DKIM savo pasirinktinį domeną, atlikite šiuos veiksmus:

- Dauguma DKIM sąrankos problemos yra susijusios su neteisingudns įrašus. Patikrinkite, ar DKIM CNAME įrašas **(ne** TXT įrašas) yra tinkamai suformatuotas. Daugiau informacijos ieškokite šioje [temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Sukūrę arba atnaujinę savo DKIM DNS įrašus domeno DNS išteklių nuomos tarnyboje (paprastai domenų registratoriuje), palaukite, kol DNS įrašai bus platinami.

- Jei negalite sukurti DKIM DNS įrašų administravimo centre, galite pakeisti \<CustomDomain\> savo pasirinktinį domeną (pvz., contoso.com) ir paleisti šią komandą ["Exchange Online PowerShell":](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
