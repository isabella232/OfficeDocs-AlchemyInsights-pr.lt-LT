---
title: Sąlyginės prieigos problemos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014886"
---
# <a name="conditional-access-issues"></a>Sąlyginės prieigos problemos

**Išspręskite prisijungimo diagnostikos problemas**

Naudodami [prisijungimo diagnostiką](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)galite greitai sužinoti, kas nutiko arba diagnozuoti problemas, susijusias su vartotojų prisijungtu:

1. Paleidžia prisijungimo diagnostiką.
1. Raskite įvykį, kurį norite analizuoti, įvesdami informaciją apie vartotoją, taikomąją programą, prisijungimo laiką, užklausos ID arba koreliacijos ID.
1. Peržiūrėkite diagnostikos rezultatus, kuriuose pateikiama išsami informacija apie tai, kas nutiko ir kokių veiksmų galite imtis, kad keistumėte (jei reikia kokių nors pasikeitimų).

**Prisijungimo trikčių šalinimo veiksmai** 

1. Pereikite į "Azure AD" prisijungimo puslapį.
1. Filtruokite prisijungimo pagal vartotoją, laiko intervalą, taikomąją programą, būseną, kliento programą ir kt.
1. Pasirinkite prisijungimo įvykį ir peržiūrėkite skirtuką sąlyginė prieiga, kad pamatytumėte, kurios strategijos buvo įvertintos.
1. Spustelėkite strategijos eilutę, kad peržiūrėtumėte išsamią informaciją apie strategiją ir suprastumėte, kodėl ji pritaikyta.

**"Sąlyginės prieigos strategijos" įrankių šalinimas**

- Tik ataskaitos režimas leidžia įvertinti strategiją netrukdant vartotojams.
- "If" įrankis leidžia imituoti prisijungimo įvykius ir peržiūrėti, kurios strategijos taikomos.
- Įžvalga ir ataskaitos darbaknygė rodo kiekvienos strategijos poveikį realiuoju laiku.

**Pradinės apsaugos strategijos**

Bazinės apsaugos strategijos pasenusios. Jie nebėra vykdomi ir netrukus bus pašalinti iš "Azure" portalo. Rekomenduojame įgalinti [saugos numatytąsias reikšmes](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Daugiau informacijos apie sąlyginę prieigą rasite:

[Geriausios "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 " sąlyginės prieigos praktikos [Sąlyginės prieigos sąlygos](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 " [Sąlyginės prieigos](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 " valdikliai [Vietos sąlygine prieiga](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
