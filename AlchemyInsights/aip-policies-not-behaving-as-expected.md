---
title: 'AIP: strategijos neveikia taip, kaip tikėtasi'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821635"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: strategijos neveikia taip, kaip tikėtasi

"Azure" informacijos apsauga: strategijos neveikia taip, kaip tikėtasi, žr. toliau pateikiamas rekomendacijas dėl įvairių strategijos problemų:

1. Jei kyla vaizdinių žymų problemų, peržiūrėkite [Kai taikomi vaizdiniai ženklai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jei kyla problemų dėl automatinio etikečių žymėjimo, peržiūrėkite Kaip sukonfigūruoti automatinio ir rekomenduojamo ["Azure"](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) informacijos apsaugos klasifikavimo sąlygas ir Kaip ieškoti [slaptos informacijos tipų.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Jei kyla problemų dėl vietinės / Pfile apsaugos, peržiūrėkite [Failų API konfigūracija](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Patikrinkite, ar naudojate aprėpties strategijas, kurios nėra tinkamai sukonfigūruotos: Kaip konfigūruoti "Azure" informacijos apsaugos strategiją konkretiems vartotojams [naudojant aprėpties strategijas.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Jei pridedant pažymėtą dokumentą "Outlook" neveikia automatinis ženklinimas, patikrinkite, ar DRMEncryptProperty nėra apibrėžtas, kaip aprašyta [čia: IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)registro saugos parametrai.

Jei vis dar kyla problemų, rinkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus prie šio kvito.

1. Atidarykite "Office" dokumentą arba sukurkite naują el. laišką programoje "Outlook".
2. Spustelėkite **Apsaugoti / slaptumo**  >  **žinyną ir atsiliepimus.**
3. Spustelėkite **Eksportuoti žurnalus.**
4. Įrašykite žurnalus į savo vietą ir pridėkite juos prie šios tarnybos užklausos.

Papildomi ištekliai:

- [Kaip konfigūruoti "Azure" informacijos apsaugos vaizdinių žymų etiketę](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Peržiūrėkite "Azure" informacijos apsaugos dokumentaciją](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Slaptumo etikečių naudojimas "Microsoft 365" programose](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

