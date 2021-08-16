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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069972"
---
# <a name="conditional-access-issues"></a>Sąlyginės prieigos problemos

**Prisijungimo diagnostikos problemų sprendimas**

Galite greitai sužinoti, kas nutiko arba diagnozuoti problemas, susijusias su vartotojo prisijungimu, naudodami [prisijungimo diagnostiką:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Paleiskite prisijungimo diagnostiką.
1. Raskite analizuojamą įvykį įvesdami išsamią informaciją apie vartotoją, taikomąją programą, prisijungimo laiką, užklausos ID arba koreliacijos ID.
1. Peržiūrėkite diagnostikos rezultatus, kuriuose rodoma išsami informacija apie tai, kas nutiko ir kokius veiksmus galite atlikti norėdami atlikti keitimus (jei reikia pakeitimų).

**Prisijungimo trikčių šalinimo veiksmai** 

1. Eikite į "Azure AD" prisijungimo puslapį.
1. Filtruokite prisijungimus pagal vartotoją, laiko diapazoną, taikomąją programą, būseną, kliento programą ir t. t.
1. Pasirinkite prisijungimo įvykį ir peržiūrėkite skirtuką Sąlyginė prieiga, kad pamatytumėte, kurios strategijos buvo įvertintos.
1. Spustelėkite strategijos eilutę, kad būtų galima peržiūrėti strategijos informaciją ir suprasti, kodėl ji taikoma.

**Įrankiai, padedai šalinti sąlyginės prieigos strategijos triktis**

- Tik ataskaitos režimas leidžia įvertinti strategiją neįvertinant vartotojų.
- "What-if" įrankis leidžia imituoti prisijungimo įvykius ir peržiūrėti, kurios strategijos taikomos.
- Įžvalgos ir ataskaitos rodo kiekvienos strategijos poveikį realiuoju laiku.

**Bazinės linijos apsaugos strategijos**

Bazinės linijos apsaugos strategijos buvo pasenusios. Jie nebetaikomi ir netrukus bus pašalinti iš "Azure" portalo. Rekomenduojame įjungti saugos [numatytąsias reikšmes](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Daugiau informacijos apie sąlyginę prieigą žr.:

[Geriausia sąlyginio prieigos "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Sąlygos sąlyginės prieigos](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Valdikliai sąlyginės prieigos](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Vietos sąlyginės prieigos](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
