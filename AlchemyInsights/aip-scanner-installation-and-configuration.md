---
title: 'AIP skaitytuvas: diegimas ir konfigūravimas'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358101"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skaitytuvas: diegimas ir konfigūravimas

**Norėdami įdiegti AIP skaitytuvą, vadovaukitės rekomenduojamomis gairėmis:**

1. Jei naujinate ir neatliekate švaraus diegimo, įsitikinkite, kad vadovavotės ["Azure" informacijos apsaugos skaitytuvo naujinimo](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) gairėmis ir vieningosios etikečių kliento versijos [naujinimo](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)gairėmis, žr.
2. Patikrinkite, ar atitinkate visus [užkardos ir tinklo infrastruktūros parametrų reikalavimus](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Įsitikinkite, kad [jūsų strategijos nustatytos](https://docs.microsoft.com/azure/information-protection/configure-policy) kaip automatinis žymėjimas arba strategijos numatytoji etiketė.
4. Įsitikinkite, kad atitinkamas failo tipas yra sukonfigūruotas etiketės/apsaugos, kaip aprašyta [failų tipai palaiko Azure informacijos apsaugos klientas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Be to, jei norite pakeisti numatytąjį veikimą, atlikite šiuos veiksmus: [Numatytojo failų apsaugos lygio keitimas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Patikrinkite, ar vartotojo abonementas, sukonfigūruotas paleisti skaitytuvo tarnybą, turi teisę pasiekti visas sukonfigūruotas saugyklas.
6. Jei vis tiek kyla problemų, eksportuokite skaitytuvo žurnalus ir pridėkite juos prie palaikymo bilieto.

**Eksportuoti Azure informacijos apsaugos skaitytuvas žurnalus**

1. Eikite į %localappdata%\Microsoft\MSIP vartotojo kontekste, kuriame veikia skaitytuvo tarnyba.
2. Zip visą turinį pagal MSIP aplanką.
3. Įrašykite žurnalus į savo vietą ir pridėkite juos prie aptarnavimo užklausos.
4. Taip pat galite naudoti [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Daugiau informacijos rasite**:
- ["Azure" informacijos apsaugos skaitytuvo diegimas automatiškai klasifikuoti ir apsaugoti failus](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Nustatyti ir naudoti atpažinimo ženklo parametras Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Aptikimo ciklo vykdymas ir skaitytuvo ataskaitų peržiūra](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- ["Azure" informacijos apsaugos dokumentų peržiūra](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- ["Azure" informacijos apsaugos reikalavimai](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Atsisiųskite "Azure" informacijos apsaugos klientą](https://www.microsoft.com/download/details.aspx?id=53018)
