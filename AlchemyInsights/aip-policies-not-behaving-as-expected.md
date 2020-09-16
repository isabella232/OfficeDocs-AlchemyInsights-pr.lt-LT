---
title: 'AIP: politika neelgiasi taip, kaip tikėtasi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663197"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politika neelgiasi taip, kaip tikėtasi

"Azure" informacijos apsauga: strategijos, kurios nėra, kaip tikėtasi, ieškokite šioje rekomenduojamų rekomendacijų įvairiose politikos srityse:

1. Jei turite problemų su vaizdiniais ženklais, peržiūrėkite, [kai taikomi vizualiniai ženklai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jei kyla problemų dėl automatinio žymėjimo, peržiūrėkite, [kaip konfigūruoti automatines ir rekomenduojamas "Azure" informacijos apsaugos sąlygas](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ir [kokie atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jei kyla problemų su prigimtine/Pfile apsauga, peržiūrėkite [failų API konfigūraciją](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Patikrinkite, ar naudojate aprėpties strategijas, kurios netinkamai sukonfigūruotos: [kaip konfigūruoti "Azure" informacijos apsaugos strategiją konkretiems vartotojams naudojant aprėpties strategijas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jei prijungus pažymėtą dokumentą "Outlook" neveikia Automatinis žymėjimas, patikrinkite, ar "DRMEncryptProperty" neapibrėžta kaip aprašyta čia: [IRM registro parametrai, skirti saugos](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jei vis dar kyla problemų, surinkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus su šiuo bilietu.

1. Atidarykite "Office" dokumentą arba sukurkite naują laišką programoje "Outlook".
2. Spustelėkite **apsaugoti/jautrumo**  >  **žinyną ir atsiliepimą**.
3. Spustelėkite **eksportuoti žurnalus**.
4. Įrašykite žurnalus į savo vietos pasirinkimą ir pridėkite juos prie šios paslaugos užklausos.

Papildomi ištekliai:

- [Kaip sukonfigūruoti "Azure" informacijos apsaugos vaizdinio žymėjimo žymę](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- ["Azure" informacijos apsaugos dokumentų peržiūra](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- ["Microsoft 365" programėlių jautrumo žymių naudojimas](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

