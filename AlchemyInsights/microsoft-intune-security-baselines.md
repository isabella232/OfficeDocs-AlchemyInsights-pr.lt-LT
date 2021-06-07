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
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793896"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius

"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius. Saugos bazinės linijos yra Windows parametrai iš anksto sukonfigūruotos grupės, naudojamos norint taikyti žinomų parametrų grupę ir numatytąsias reikšmes, kurias rekomenduoja atitinkamos saugos komandos. Sukurdami saugos bazinį profilį "Intune", sukuriate šabloną, kurį sudaro keli įrenginio konfigūracijos profiliai.

Kai diegiate saugos bazines linijas vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, veikiaems Windows 10 arba naujesnėse versijose. Pvz., "Microsoft" mobiliųjų įrenginių valdymo (MDM) saugos bazinė linija automatiškai įgalina ""BitLocker"" keičiamiesiems diskams, reikalingas įrenginio atrakinimo slaptažodis ir išjungiamas bazinis autentifikavimas. Kai numatytoji reikšmė neveikia jūsų aplinkoje, galite tinkinti bazinę liniją, kad pritaikytų norimus parametrus.

Saugos bazinės linijos taip pat padeda sukurti saugią darbo eigą Microsoft 365. Saugos bazinė linija apima geriausias saugos parametrų praktikas ir rekomendacijas. Intune partners with the Windows team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.

Jei tik pradedate naudoti "Intune" ir neįtikite, kur pradėti, saugos bazinės linijos padeda greitai sukurti ir įdiegti saugų profilį. Jei šiuo metu naudojate grupės strategiją, perkelti į "Intune" valdymo tikslais yra daug lengviau naudojant saugos bazines linijas, nes jos integruotos į "Intune" ir apima pažangiausias valdymo galimybes.

Norėdami sužinoti daugiau, [žr. Windows bazinės linijos](/windows/security/threat-protection/windows-security-baselines) ir [mobiliųjų įrenginių valdymas.](/windows/client-management/mdm/)

