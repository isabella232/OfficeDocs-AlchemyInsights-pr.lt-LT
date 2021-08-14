---
title: DKIM sąrankos problemų sprendimas
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945939"
---
# <a name="fix-dkim-setup-issues"></a>DKIM sąrankos problemų sprendimas

Jei kyla problemų įgalinus DKIM pasirinktiniam domenui, atlikite šiuos veiksmus:

- Dauguma DKIM sąrankos problemų yra susijusios su netinkamais DNS įrašais. Patikrinkite, ar tinkamai suformatuotas DKIM CNAME įrašas **(ne** TXT įrašas). Daugiau informacijos žr. šioje [temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Sukūrę arba atnaujinę DKIM DNS įrašus savo domeno DNS išteklių nuomos paslaugoje (paprastai domeno registratorius), palaukite, kol bus išplatinti DNS įrašai.

- Jei negalite sukurti DKIM DNS įrašų administravimo centre, galite pakeisti pasirinktinį domeną (pvz., "contoso.com") ir vykdyti šią komandą \<CustomDomain\> ["Exchange Online PowerShell":](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
