---
title: Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104352"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius

"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius. Saugos bazinės linijos Windows parametrų iš anksto sukonfigūruotos grupės, naudojamos žinomų parametrų grupei ir numatytosios reikšmės, kurias rekomenduoja atitinkamos saugos komandos, taikyti. Sukurdami saugos bazinį profilį "Intune", sukuriate šabloną, kurį sudaro keli įrenginio konfigūracijos profiliai.

Kai diegiate saugos bazines linijas vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, veikiaems Windows 10 arba naujesnėse versijose. Pvz., "MDM Security Baseline" automatiškai (1) įgalina "BitLocker" keičiamuose diskuose, (2) reikalauja slaptažodžio įrenginiui atrakinti, o (3) išjungia bazinį autentifikavimą. Kai numatytoji reikšmė neveikia jūsų aplinkoje, tinkinkite bazinę liniją, kad pritaikytų norimus parametrus.

Saugos bazinės linijos taip pat padeda sukurti saugią darbo eigą Microsoft 365. Toliau pateikiami keli šio pranašumo pranašumai:

- Saugos bazinė linija apima geriausias saugos parametrų praktikas ir rekomendacijas. Kadangi "Intune" partneriai su Windows komanda, kuri sukuria grupių strategijų bazines linijas, šios rekomendacijos pagrįstos išsamiomis rekomendacijomis ir išsamia patirtimi.
- Jei esate naujas "Intune" ir neįtikite, kur pradėti, saugos bazinės linijos padės greitai sukurti ir įdiegti saugų profilį.
- Jei šiuo metu naudojate grupės strategiją, tada perkelti į "Intune" valdymo tikslais yra daug lengviau naudojant saugos bazines linijas, nes jos integruotos į "Intune" ir apima pažangiausias valdymo galimybes.

Norėdami sužinoti daugiau, [žr. Windows bazinės linijos](https://go.microsoft.com/fwlink/?linkid=2141503) ir [mobiliųjų įrenginių valdymas.](https://go.microsoft.com/fwlink/?linkid=2141701)