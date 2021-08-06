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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999680"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Įspėjimo el. laiškai iš "Phish Delivered due to tenant or user override" strategijos

Numatytoji įspėjimo strategija, pavadinta "Phish Delivered due to tenant or user override" (apsimetant pristatyta dėl nuomotojo arba vartotojo perrašymo), buvo išsamūs nuomotojams su "Microsoft" sargyba, skirta "Office 365 P1" ir "P2" licencijoms. Jei gavote šį įspėjimą, toliau pateikiami veiksmai, kuriuos reikia atlikti:

1. Įspėjimo pranešime spustelėkite Peržiūrėti **įspėjimą,** kad pereidami **į** saugos ir saugos & puslapį.

2. Pasirinkite įspėjimą, kad pamatytumėte parinktį **Peržiūrėti pranešimų sąrašą arba** Peržiūrėti **pranešimus naršyklėje**. Abi šios parinktys pereis prie pranešimo išsamios informacijos, kurioje yra pranešimo ID. Atkreipkite dėmesį, kad "Threat Explorer" saitas automatiškai filtruoja pranešimus, kurie atitinka įspėjimo kriterijus. Gali tekti koreguoti datos filtrą grėsmių naršyklėje.

Sukčiavimo apsimetant pranešimas buvo pristatytas dėl rankiniu būdu sukonfigūruoto perrašymo:

- Vartotojo nustatytas leistinas siuntėjas arba domenas.

- Leistinas siuntėjas arba domenas, administratoriaus nustatytas apsaugos nuo pašto šiukšlių politikoje.

- Leidžiamas IP adresas ryšio filtro politikoje.

- Pašto srauto taisyklė (dar vadinama transportavimo taisykle), sukonfigūruota leisti pranešimus.

Jei manote, kad pranešimas buvo neteisingai pažymėtas kaip sukčiavimas apsimetant, naudokite Outlook [ataskaitos pranešimo papildinį, kad](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) pateiktų pranešimo pavyzdžius "Microsoft".
