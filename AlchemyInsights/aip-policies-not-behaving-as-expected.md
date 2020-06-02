---
title: 'AIP: Politika neveikia taip, kaip tikėtasi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506566"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politika neveikia taip, kaip tikėtasi

Azure informacijos apsauga: strategijos neveikia kaip tikėtasi, ieškokite rekomenduojamų gairių įvairių strategijos problemų:

1. Jei kyla problemų dėl vaizdinių ženklų, peržiūrėkite [Kai taikomi vaizdiniai ženklai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jei kyla problemų dėl automatinio ženklinimo, peržiūrėkite [Kaip konfigūruoti automatinio ir rekomenduojamo "Azure" informacijos apsaugos ir](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ["What the sensitive information types" klasifikavimo](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)sąlygas .
3. Jei kyla problemų dėl apsaugos nuo vietinio / Pfailo, peržiūrėkite [failo API konfigūraciją](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Patikrinkite, ar naudojate aprėpties strategijas, kurios nėra tinkamai sukonfigūruotos: [kaip konfigūruoti konkrečių vartotojų Azure informacijos apsaugos strategiją naudojant aprėpties strategijas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jei automatinis žymėjimas neveikia programoje "Outlook" pridedant pažymėtą dokumentą, patikrinkite, ar DRMEncryptProperty nėra apibrėžta kaip aprašyta čia: [IRM registro parametrus saugos](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jei vis tiek kyla problemų, rinkkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus prie šio bilieto.

1. Atidarykite "Office" dokumentą arba sukurkite naują el. laišką programoje "Outlook".
2. Spustelėkite **Apsaugoti / jautrumas**  >  **Žinynas ir atsiliepimai**.
3. Spustelėkite **Eksportuoti žurnalus**.
4. Įrašykite žurnalus į savo vietą ir pridėkite juos prie šios tarnybos užklausos.

Papildomi ištekliai:

- [Kaip sukonfigūruoti žymę visual pažymi Azure informacijos apsauga](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- ["Azure" informacijos apsaugos dokumentų peržiūra](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Jautrumo etikečių naudojimas "Office" programose](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

