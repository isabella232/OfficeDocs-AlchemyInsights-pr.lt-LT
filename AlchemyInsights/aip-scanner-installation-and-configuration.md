---
title: 'AIP skaitytuvas: diegimas ir konfigūravimas'
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
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934265"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skaitytuvas: diegimas ir konfigūravimas

**Norėdami įdiegti AIP skaitytuvą, vadovaukitės rekomenduojamomis rekomendacijomis:**

1. Jei naujinate versiją ir neįrengite švaraus diegimo, įsitikinkite, kad laikėsite ["Azure"](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) informacijos apsaugos skaitytuvo versijos naujinimo ir vieningo etikečių kliento rekomendacijų, žr. ["Azure" informacijos apsaugos skaitytuvo versijos naujinimas.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Patikrinkite, ar atitinkate visus [užkardos ir tinklo infrastruktūros parametrų reikalavimus.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. [Įsitikinkite, kad strategijos nustatytos](https://docs.microsoft.com/azure/information-protection/configure-policy) kaip automatinis ženklinimas arba strategijos numatytoji etiketė.
4. Įsitikinkite, kad atitinkamas failo tipas sukonfigūruotas naudoti etiketę / apsaugą, kaip aprašyta failų [tipuose, kuriuos palaiko "Azure" informacijos apsaugos klientas.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Be to, jei norite pakeisti numatytąjį veikimą, vadovaukitės šiomis gairėmis: [Numatytojo failų apsaugos lygio keitimas.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Patikrinkite, ar vartotojo paskyra, sukonfigūruota vykdyti skaitytuvo tarnybą, turi teises pasiekti visas sukonfigūruotas saugyklas.
6. Jei vis tiek kyla problemų, eksportuokite skaitytuvo žurnalus ir įtraukite juos į palaikymo kvitą.

**"Azure" informacijos apsaugos skaitytuvo žurnalų eksportavimas**

1. Eikite į %localappdata%\Microsoft\MSIP pagal vartotojo kontekstą, kuriame veikia skaitytuvo tarnyba.
2. Suglaudinkite visą turinį po MSIP aplanku.
3. Įrašykite žurnalus į savo vietą ir pridėkite juos prie savo tarnybos užklausos.
4. Taip pat galite naudoti [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Papildomos informacijos žr.:**
- ["Azure" informacijos apsaugos skaitytuvo diegimas norint automatiškai klasifikuoti ir apsaugoti failus](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication parametro Atpažinimo ženklas nurodymas ir naudojimas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Aptikimo ciklo paleidimas ir skaitytuvo ataskaitų peržiūra](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Peržiūrėkite "Azure" informacijos apsaugos dokumentaciją](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- ["Azure" informacijos apsaugos reikalavimai](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Atsisiųsti "Azure" informacijos apsaugos klientą](https://www.microsoft.com/download/details.aspx?id=53018)
