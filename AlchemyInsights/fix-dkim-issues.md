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
# <a name="fix-dkim-setup-issues"></a>DKIM sąrankos problemų sprendimas

Jei kyla nesklandumų, leidžianti DKIM pasirinktinio domeno, atlikite šiuos veiksmus:

- Dauguma DKIM nustatymo problemos yra susijusios su neteisingas DNS įra us. Patikrinkite, ar teisingai suformatuotas DKIM CNAME įrašą (**ne** TXT įrašą). Norėdami gauti daugiau informacijos, peržiūrėkite šią [temą](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Po to, kai sukurti arba atnaujinti savo DKIM DNS įra us DNS išteklių nuomos tarnybos domeno (paprastai domenų registratoriaus), palaukti, kol DNS įrašai platinti.

- Jei jūs negalite sukurti DKIM DNS įrašų administravimo centro, jūs galite pakeisti \<CustomDomain\> su savo individualiame domene (pvz.,.: contoso.com) ir vykdykite šią komandą į [Exchange Online "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
