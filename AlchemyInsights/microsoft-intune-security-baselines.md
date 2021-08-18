---
title: Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331993"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius

"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius. Saugos bazinės linijos yra Windows parametrai iš anksto sukonfigūruotos grupės, naudojamos žinomų parametrų grupei ir numatytosios reikšmės, kurias rekomenduoja atitinkamos saugos komandos, taikyti. Sukurdami saugos bazinį profilį "Intune", sukuriate šabloną, kurį sudaro keli įrenginio konfigūracijos profiliai.

Kai diegiate saugos bazines linijas vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, veikiaems "Windows 10 arba naujesnėse versijose. Pvz., "Microsoft" mobiliųjų įrenginių valdymo (MDM) saugos bazinė linija automatiškai įgalina "BitLocker" keičiamiesiems diskams, reikalauja slaptažodžio įrenginiui atrakinti ir išjungia bazinį autentifikavimą. Kai numatytoji reikšmė neveikia jūsų aplinkoje, galite tinkinti bazinę liniją, kad pritaikytų norimus parametrus.

Saugos bazinės linijos taip pat padeda sukurti "end-to-end" saugią darbo eigą Microsoft 365. Saugos bazinė linija apima geriausias saugos parametrų praktikas ir rekomendacijas. Intune partners with the Windows team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.

Jei tik pradedate naudoti "Intune" ir neįtikite, kur pradėti, saugos bazinės linijos padeda greitai sukurti ir įdiegti saugų profilį. Jei šiuo metu naudojate grupės strategiją, perkelti į "Intune" valdymo tikslais yra daug lengviau naudojant saugos bazines linijas, nes jos integruotos į "Intune" ir apima pažangiausias valdymo galimybes.

Norėdami sužinoti daugiau, [žr. Windows bazinės linijos](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) ir [mobiliųjų įrenginių valdymas.](https://docs.microsoft.com/windows/client-management/mdm/)

