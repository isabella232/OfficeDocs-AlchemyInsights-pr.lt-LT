---
title: "\"Microsoft\" sargybos, kurios galinis taškas yra \"Linux\", našumo problemos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794004"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>"Microsoft" sargybos, kurios galinis taškas yra "Linux", našumo problemos

Šiame straipsnyje aprašomi veiksmai, kaip nustatyti "Microsoft Defender for Endpoint" veikimo problemas "Linux".

Pirmiausia svarbu patikrinti, ar problema, su kuriomis susiduriate, išspręsta naudojant naujausią [versiją.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Norėdami pradėti tyrimą, žr. ["Microsoft Defender for Endpoint" veikimo trikčių šalinimas "Linux".](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Išimtys

Išimtys gali padėti sumažinti našumo problemas. Prieš pradėdami peržiūrėkite savo išimtis, kad būtų žinoma ir dokumentuota papildoma rizika.

Daugiau informacijos žr. "Microsoft Defender [for Endpoint" išimčių konfigūravimas ir tikrintas "Linux".](/microsoft-365/security/defender-endpoint/linux-exclusions)

Jei turite kelis failus& kuriuos norite pašalinti, ir jie visi yra tame pačiame mountpoint, gali būti lengviau pašalinti mountpoint. Nuo vasario leidimo 101.22.80 galite neįtraukti viso kalno taško.

Pvz., jei /mnt/backup yra mountpoint, galite įtraukti /mnt/backup į neįtrauktų sąrašą vykdydami šią komandą:

`$ mdatp exclusion folder add –path /mnt/backup`

**Pastaba:** įtraukus išimtis padidėja pavojus, kad nebus aptikta kenkėjiškų programų, todėl jos turėtų būti tvarkomos ir įgyvendinamos atsargiai.

## <a name="need-help"></a>Reikia pagalbos?

Norėdami jums padėti efektyviausiu būdu, prieš atidarydami palaikymo bylą, surinkite diagnostikos duomenis.
