---
title: Autentifikavimo programa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082950"
---
# <a name="authentication-app"></a>Autentifikavimo programa

Jei esate visuotinis administratorius, naudodami prisijungimo diagnostiką galite greitai sužinoti, kas nutiko arba nustatyti problemas, susijusias [su vartotojo prisijungimu.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Pradėkite diagnostiką spustelėdami mygtuką[Paleisti diagnostiką.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Raskite analizuojamą įvykį įvesdami išsamią informaciją apie vartotoją, taikomąją programą, prisijungimo laiką, užklausos ID arba koreliacijos ID.
1. Peržiūrėkite diagnostikos rezultatus, kuriuose rodoma išsami informacija apie tai, kas nutiko ir kokius veiksmus galite atlikti, jei reikia atlikti keitimus.

**Patikrinkite taikomą scenarijų:**

1. Jei vartotojas negaus "push" pranešimo "Microsoft Authenticator programėlėje, patikrinkite, ar jie nerodomas pagal MFA užblokuotus vartotojus, kaip aprašyta skyriuje Vartotojų blokavimas [ir atblokavimas](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Jei vartotojas nėra užblokuotas MFA, bet negauna "push" pranešimo, jis gali atidaryti "Microsoft Authenticator" programą, kuri išims laukiančias patvirtinimo užklausas.
1. Kaip alternatyvus prisijungimo būdas, vartotojas taip pat gali spustelėti Prisijungti kitu būdu ir pasirinkti naudoti patvirtinimo kodą iš mano mobiliųjų įrenginių programėlės.
1. "Microsoft Authenticator" programa yra vienintelis būdas, kurį gali naudoti daugelis vartotojų. [Sužinokite daugiau apie saugos numatytąsias](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)reikšmes , [Authenticator programėlių DUK](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) apie dažniausiai užduodamus klausimus ir kaip juos išspręsti.
 
**Rekomenduojami vaizdo įrašai**

[Kaip nustatyti "Authenticator programėlę naujame telefone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
