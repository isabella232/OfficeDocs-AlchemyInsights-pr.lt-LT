---
title: "\"Microsoft Defender\", skirtas \"Office 365\" apsaugos nuo sukčiavimo apsimetant strategijai"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695635"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>"Microsoft Defender", skirtas "Office 365" apsaugos nuo sukčiavimo apsimetant strategijai

Šie parametrai įgalina strategiją, vadinamą *domenu ir generaliniu direktoriumi*. Ši strategija suteikia ir vartotojo, ir domeno apsaugą nuo apsimetimas ir tada taiko strategiją visiems pašto vartotojams, kuriuos gavo domenas. Pirmiausia įtraukite šią informaciją, kad sukurtumėte strategiją:

- **Pavadinimas**: domain ir CEO **Description**: užtikrina, kad generalinis direktorius ir jūsų domenas nebus apsimečiami.
  **Pritaikyta**: pasirinkite **gavėjo domeną**. Dalyje **bet kurį iš šių** pasirinkite **pasirinkti**, tada pasirinkite domeną. Pasirinkite **+ įtraukti**. Pažymėkite žymės langelį, esantį prie domeno vardo sąraše (pvz., *contoso.com*), tada pasirinkite **įtraukti**. Pasirinkite **atlikta**.
- Kai strategija bus sukurta, galite pakoreguoti strategiją naudodami šias parinktis:
  - **Vartotojų įtraukimas į apsaugą:** Šiame pavyzdyje, bent minimaliai įtraukite generalinio direktoriaus elektroninio pašto adresą.
  - **Įtraukite domenus, kad apsaugotumėte**: įtraukite organizacijos domeną, kuriame yra generalinio direktoriaus biuras.
  - **Pasirinkite veiksmai**: **Jei laišką siunčia apsimestas vartotojas**, pasirinkite **Peradresuoti pranešimą į kitą elektroninio pašto adresą**, tada įveskite saugos administratoriaus el. pašto adresą (pvz., *securityadmin@contoso.com*). **Jei el. laišką siunčia apsimestas domenas**, pasirinkite **sulaikyti pranešimą**.
  - **Pašto dėžutės informacijos**: pagal numatytuosius nustatymą Ši parinktis pažymėta, kai kuriate naują apsaugos nuo sukčiavimo apsimetant strategiją. Palikite **šį parametrą,** kad būtų pasiekti Geriausi rezultatai.
  - **Patikimų siuntėjų ir domenų įtraukimas:** Šiame pavyzdyje negalima apibrėžti jokių perrašymų.
- Peržiūrėjus parametrus, pasirinkite **Kurti šią strategiją** arba **įrašyti**, jei reikia.

Norėdami sužinoti daugiau, peržiūrėkite [apsaugos nuo sukčiavimo apsimetant strategijas programoje "Microsoft 365"](https://go.microsoft.com/fwlink/?linkid=2092235).
