---
title: "\"Microsoft\" sargybos Office 365 apsaugos nuo sukčiavimo apsimetant strategijos pavyzdys"
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035014"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>"Microsoft" sargybos Office 365 apsaugos nuo sukčiavimo apsimetant strategijos pavyzdys

Šie parametrai įgalina strategiją, vadinamą *Domenas ir vadovas*. Ši strategija suteikia tiek vartotojo, tiek domeno apsaugą nuo apsimetimo ir tada taiko strategiją visiems el. laiškams, kuriuos gauna vartotojai iš domeno. Pirmiausia įtraukite šią informaciją, kad sukurtumėte strategiją:

- **Pavadinimas**: Domenas ir vadovas **Aprašas**: Užtikrina, kad direktorius ir jūsų domenas nebūtų apsimesti.
  **Taikoma**: pasirinkite **Gavėjo domenas yra**. Dalyje **Bet kuris iš šių** pasirinkite **Pasirinkti**, tada pasirinkite domeną. Pasirinkite **+ Įtraukti**. Pažymėkite žymės langelį šalia sąraše domeno vardo (pvz., *contoso.com*), tada pasirinkite **Įtraukti**. Pasirinkite **Atlikta**.
- Sukūrus strategiją, galite pakoreguoti strategiją naudodami šias parinktis:
  - **Įtraukite vartotojų, kad apsaugotumėte:** Šiame pavyzdyje įtraukite bent ceo el. pašto adresą.
  - **Įtraukite domenų, kad** apsaugotumėte: įtraukite organizacijos domeną, kuriame yra ceo biuras.
  - **Pasirinkite veiksmai**: Jei **el.** laišką siunčia apsimestas vartotojas , pasirinkite Peradresuoti laišką kitu el. pašto adresu **,** tada įveskite saugos administratoriaus el. pašto adresą (pvz., *securityadmin@contoso.com*). Jei **el. laišką siunčia apsimestas domenas,** pasirinkite **Sulaikyti pranešimą**.
  - **Pašto dėžutės informacija:** pagal numatytuosius nustatymus ši parinktis pasirenkama kuriant naują sukčiavimo apsimetant strategiją. Palikite šį **parametrą Į,** kad būtų pasiekti geriausi rezultatai.
  - **Patikimų siuntėjų ir domenų įtraukimas:** Šiame pavyzdyje nenu apibrėžkite perrašymo.
- Peržiūrėsite parametrus, pasirinkite Kurti **šią strategiją** arba **Įrašyti**, jei reikia.

Norėdami sužinoti daugiau, [žr. Apsaugos nuo sukčiavimo apsimetant strategijos Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
