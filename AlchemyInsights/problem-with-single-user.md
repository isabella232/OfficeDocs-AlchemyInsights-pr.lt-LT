---
title: Problema su vienu vartotoju
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430200"
---
# <a name="problem-with-single-user"></a>Problema su vienu vartotoju

- Vartotojas gali būti nesukonfigūruotas, nes tarnyba dar neturėjo galimybės įvertinti vartotojo. Peržiūrėkite nurodymus, kaip ilgai trunka parengimas, taip pat ir eigos juostos parengimo konfigūravimo puslapyje. Jei stabili būsena, nurodyta sekcijoje papildoma informacija, yra prieš vartotojo sukūrimo/atnaujinimo/panaikinimo datą, tai reiškia, kad dar neįvertinome vartotojo. Pagal šį scenarijų, geriausia, ką reikia padaryti – palaukite, kol bus baigta parengimo tarnyba.

  - Atkreipkite dėmesį, kad mūsų paslauga yra tik apie vartotojų pakeitimą šaltinio sistemoje (debesies HR). "Azure AD" šaltinio sistemoje turi būti galiojantis keitimas, kad būtų galima aptikti keitimą ir srautą į "Active Directory".
- Parengimo tarnyba vertino vartotoją ir nustatė, kad jis neturėtų būti konfigūruojamas:
  - Jei nustatėte atributą pagal aprėpties filtrą, įsitikinkite, kad vartotojas atitinka nurodytus kriterijus.
  - Jei vartotojai jau yra tikslinėse sistemose ir vartotojo būsena šaltinio ir paskirties atitikmuo, mes nesiimsime jokių tolesnių veiksmų.
- Parengimo tarnyba bandė pateikti vartotojui ir nepavyko. Šiuose scenarijuose Peržiūrėkite parengimo žurnalų skirtuką trikčių diagnostika ir rekomendacijos:
  - Vartotojui būtinas atributas gali trūkti vietiniame "Active Directory" arba "Azure AD". Pvz., "userPrincipalName" arba "Samaccountiname" generavimo taisyklės nesugeneruoja tinkamos reikšmės.
  - Sutampantis atributas (paprastai darbuotojai) nėra skirtas unikaliam vartotojui vietinėje "Active Directory" arba "Azure AD". Pvz., "AD" yra du vartotojai su tuo pačiu darbuotojai ir Tarnyba pateikia klaidos kodą, nurodantį to paties šaltinio įrašo dublikatus paskirties įrašus.

Norėdami peržiūrėti vieno vartotojo ir grupių žurnalus, peržiūrėkite [konkretaus vartotojo problemų parengimo žurnalus](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
