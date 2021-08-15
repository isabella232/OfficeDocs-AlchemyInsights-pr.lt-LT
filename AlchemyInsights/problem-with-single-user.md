---
title: Vieno vartotojo problema
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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960159"
---
# <a name="problem-with-single-user"></a>Vieno vartotojo problema

- Vartotojas gali būti nesuteikite, nes tarnyba dar neturėjo galimybės įvertinti vartotojo. Peržiūrėkite rekomendacijas, kiek laiko trunka parengimas, ir eigos juostą parengimo konfigūravimo puslapyje. Jei pastovi būsena, nurodyta papildomos išsamios informacijos skyriuje, yra prieš datą, kai vartotojas buvo sukurtas / atnaujintas / panaikintas, tai reiškia, kad dar neįvertinome vartotojo. Pagal šį scenarijų geriausia palaukti, kol baigsis parengimo tarnyba.

  - Atkreipkite dėmesį, kad mūsų tarnyba žino tik apie pakeitimus vartotojams šaltinio sistemoje (debesies HR). Turi būti galiojantis "Azure AD" šaltinio sistemos pakeitimas, kad būtų galima aptikti pakeitimą ir tekėti į "Active Directory".
- Parengimo tarnyba įvertinė vartotoją ir nustatė, kad ji neturėtų būti parengimo:
  - Jei nustatėte atributu pagrįstą filtravimo filtrą, įsitikinkite, kad vartotojas atitinka jūsų nurodytus kriterijus.
  - Jei vartotojai jau yra paskirties sistemoje, o vartotojo būsena šaltinio ir paskirties atitikmenyje, mes nesiimsime jokių tolesnių veiksmų.
- Parengimo tarnyba bandė parengti vartotoją ir ji nepavyko. Šių scenarijų atveju peržiūrėkite parengimo žurnalų skirtuką Trikčių šalinimas ir rekomendacijos:
  - Vietinėje "Active Directory" arba "Azure AD" gali trūkti būtinojo atributo vartotojui. Pvz., userPrincipalName arba sAMAccountName generavimo taisyklės negeneruoja reikiamos reikšmės.
  - Atitinkantis atributas (paprastai employeeId) nėra skirtas unikaliam vartotojui vietiniame "Active Directory" arba "Azure AD". Pvz., AD yra du vartotojai, kurių darbuotojo Id yra tas pats, o tarnyba pateikia klaidos kodą, nurodantį pasikartojančius to paties šaltinio įrašo tikslinius įrašus.

Norėdami peržiūrėti vieno vartotojo ir grupių žurnalus, žr. Konkretaus vartotojo problemos parengimo [žurnalų peržiūra.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
