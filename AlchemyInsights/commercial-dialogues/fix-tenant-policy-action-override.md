---
title: Nuomotojo strategijos taisymas (veiksmų perrašymo)
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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896083"
---
# <a name="fix-tenant-policy-action-override"></a>Nuomotojo strategijos taisymas (veiksmų perrašymo)

Vienas iš jūsų apsaugos nuo pašto šiukšlių strategijų paveikė šį pranešimą. Norėdami peržiūrėti strategijas, atlikite šiuos veiksmus:

1. ""Microsoft 365" sargyba" portale eikite į El. & bendradarbiavimo <https://security.microsoft.com/> strategijos &  \> **Taisyklės** \> **Grėsmių** \>   strategijos Apsauga nuo pašto šiukšlių skyriuje Strategijos.

   Norėdami pereiti tiesiai į apsaugos **nuo pašto šiukšlių strategijų** puslapį, naudokite <https://security.microsoft.com/antispam> .

2. Puslapyje **Apsaugos nuo pašto** šiukšlių strategijos pasirinkite strategiją spustelėdami strategijos pavadinimą (**Tipas** yra Pasirinktinis **apsaugos nuo** pašto šiukšlių strategija arba **Pavadinimas** yra **"Anti-Spam" gavimo strategija (numatytoji)**).
3. Rodomame išsamios informacijos iškeliame lange pasirinkite **Redaguoti** veiksmus **dalyje** Veiksmai.
4. Sekcijoje **Pranešimo veiksmai** peržiūrėkite pašto **šiukšlių,** didelio patikimumo pašto šiukšlių  **,** sukčiavimo apsimetant ir didelio patikimumo apsimetant nuosprendį, kad pamatytumėte, ar pasirinkta kuri nors iš šių reikšmių:
   - **X antraštės įtraukimas**
   - **Iš anksto atidarytas temos eilutė su tekstu**
   - **Peradresuoti laišką į el. pašto adresą**
   - **Naikinti pranešimą**
   - **Jokių veiksmų**

   Gali būti, kad standartiniai parametrai **taikomi visiems** vartotojams Exchange Online Protection paveikė pranešimą.

Daugiau informacijos žr. [Apsaugos nuo pašto šiukšlių strategijų konfigūravimas EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
