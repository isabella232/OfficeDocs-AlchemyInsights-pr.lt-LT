---
title: 2491 Įspėjimo el. laiškai iš strategijos "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316366"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Įspėjimo el. laiškai iš "Phish Delivered due to tenant or user override" strategijos

Numatytoji įspėjimo strategija, pavadinta Apsimestinių duomenų pristatymo dėl nuomotojo arba vartotojo **perrašymo, pasiekiama organizacijose,** kuriose yra "Microsoft" sargybos Office 365 P1 ir P2 licencijų. Jei gavote šį įspėjimą, toliau pateikiami veiksmai, kuriuos reikia atlikti:

1. Įspėjimo pranešime spustelėkite Peržiūrėti **įspėjimą,** kad pereidami **į** puslapį Įspėjimai "Microsoft 365" sargyba portale.

2. Pasirinkite įspėjimą, kad pamatytumėte parinktį **Peržiūrėti pranešimų sąrašą arba** Peržiūrėti **pranešimus naršyklėje**. Abi šios parinktys pereis prie pranešimo išsamios informacijos, kurioje yra pranešimo ID. Atkreipkite dėmesį, kad "Threat Explorer" saitas automatiškai filtruoja pranešimus, kurie atitinka įspėjimo kriterijus. Gali tekti koreguoti datos filtrą grėsmių naršyklėje.

Sukčiavimo apsimetant pranešimas buvo pristatytas dėl rankiniu būdu sukonfigūruoto perrašymo:

- Vartotojo nustatytas leistinas siuntėjas arba domenas.
- Leistinas siuntėjas arba domenas, administratoriaus nustatytas apsaugos nuo pašto šiukšlių politikoje.
- Leidžiamas IP adresas ryšio filtro politikoje.
- Pašto srauto taisyklė (dar vadinama transportavimo taisykle), sukonfigūruota leisti pranešimus.

Jei manote, kad pranešimas neteisingai pažymėtas kaip sukčiavimas apsimetant, naudokite [administratoriaus pateikimą,](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) kad pranešimas būtų pateiktas "Microsoft".

Vartotojai gali naudoti ataskaitos [pranešimo papildinį arba "Report Phishing"](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) papildinį Outlook pateikti pranešimų pavyzdžius "Microsoft".
