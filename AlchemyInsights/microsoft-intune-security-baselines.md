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
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098070"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius

"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius. Saugos bazinės linijos yra Windows parametrai iš anksto sukonfigūruotos grupės, naudojamos norint taikyti žinomų parametrų grupę ir numatytąsias reikšmes, kurias rekomenduoja atitinkamos saugos komandos. Sukurdami saugos bazinį profilį "Intune", sukuriate šabloną, kurį sudaro keli įrenginio konfigūracijos profiliai.

Kai diegiate saugos bazines linijas vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, veikiaems Windows 10 arba naujesnėse versijose. Pvz., "Microsoft" mobiliųjų įrenginių valdymo (MDM) saugos bazinė linija automatiškai įgalina "BitLocker" keičiamiesiems diskams, reikalauja slaptažodžio įrenginiui atrakinti ir išjungia bazinį autentifikavimą. Kai numatytoji reikšmė neveikia jūsų aplinkoje, galite tinkinti bazinę liniją, kad pritaikytų norimus parametrus.

Saugos bazinės linijos taip pat padeda sukurti saugią darbo eigą Microsoft 365. Saugos bazinė linija apima geriausias saugos parametrų praktikas ir rekomendacijas. Intune partners with the Windows team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.

Jei tik pradedate naudoti "Intune" ir neįtikite, kur pradėti, saugos bazinės linijos padeda greitai sukurti ir įdiegti saugų profilį. Jei šiuo metu naudojate grupės strategiją, perkelti į "Intune" valdymo tikslais yra daug lengviau naudojant saugos bazines linijas, nes jos integruotos į "Intune" ir apima pažangiausias valdymo galimybes.

Norėdami sužinoti daugiau, [žr. Windows bazinės linijos](/windows/security/threat-protection/windows-security-baselines) ir [mobiliųjų įrenginių valdymas.](/windows/client-management/mdm/)

