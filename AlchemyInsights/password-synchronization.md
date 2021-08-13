---
title: Slaptažodžių sinchronizavimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960843"
---
# <a name="password-synchronization"></a>Slaptažodžių sinchronizavimas

**Slaptažodžių hash sinchronizavimas iš viso neveikia**

Kai kurios dažniausios problemos, su kuriomis susiduria klientai, kai neveikia slaptažodžių hash sinchronizavimas:

- "Active Directory" paskyrai, kurią "Azure AD Prisijungimas" naudoja bendrauti  su vietinę  "Active Directory", nėra suteikta replikuoti katalogų pakeitimus ir replikuoti katalogų pakeitimus Visos teisės, būtinos norint sinchronizuoti slaptažodžius – turite tai ištaisyti suteikdami šias teises "Active Directory" paskyrai.
- Slaptažodžių hash sinchronizavimas išjungiamas, kai administratorius  pakeitė "User Sign-In" metodą iš slaptažodžių sinchronizavimo į kitą parinktį, pvz., susiejimą su **AD FS** "Azure AD Prisijungimas" vediklio – tai galite išspręsti iš naujo įgalinę slaptažodžio **hash sinchronizavimo** funkciją "Azure AD Prisijungimas" vediklio.
- Ryšio su vietinę "Active Directory" problema. Pvz., kai kurie domeno valdikliai nepasiekiami "Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Prisijungimas" arba būtini prievadai blokuojami užkardos – tai reikia išspręsti užtikrinant, kad ryšys tarp "Azure AD Prisijungimas" serverio ir vietinės "Active Directory" veiktų tinkamai.
- "Azure AD Prisijungimas" serveris šiuo metu yra sustojimo režimu, todėl serveris negalės naudoti slaptažodžių sąsagų – norėdami išspręsti šią problemą, atlikite veiksmus, aprašytus skyriuje Slaptažodžių sinchronizavimo trikčių šalinimas [naudojant "Azure AD Prisijungimas" sinchronizavimą –](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)slaptažodžiai nesinchronizuojami .

**Slaptažodžių hash sinchronizavimas neveikia kai kuriems mano vartotojams**

1. Jei pastebėjote, kad vartotojo slaptažodžių hash nesinchronizuojama, naudokite "Azure AD Prisijungimas" trikčių šalinimo užduotį, kad ištirtų ir išspręstų problemą.  Atlikite šias užduotis:

    a. [Trikčių diagnostikos užduoties paleidimas vedlyje](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Trikčių diagnostikos "cmdlet" naudojimas norint ištirti slaptažodžio sinchronizavimo problemą naudojant konkretų naudojimą](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Vietinis "Active Directory" vartotojo objektas įgalintas, kad **vartotojas turi pakeisti slaptažodį kitą kartą prisiregistravus.** Įgalinus šią parinktį, vartotojui priskiriamas laikinas slaptažodis ir jis bus paragintas pakeisti slaptažodį kitame prisijungime. "Azure AD Prisijungimas" nesinchronizuoja laikinųjų slaptažodžių su "Azure AD".

Norėdami išspręsti šią problemą, atlikite vieną iš šių užduočių:

- Paprašykite vartotojo prisijungti prie vietinės programos (pvz., Windows darbalaukio) ir pakeisti slaptažodį. Naujas slaptažodis bus sinchronizuotas su "Azure AD".
- Administratoriaus atnaujinkite vartotojo slaptažodį neįjungdami parinkties Vartotojas turi pakeisti slaptažodį kitą kartą prisijungdami **ir** bendrinti naują slaptažodį su vartotojas.

3. Vietinis "Active Directory" vartotojo objektas netinkamai **sukonfigūruotas objektų sinchronizavimui** arba slaptažodžių sinchronizavimui. Norėdami išspręsti šią problemą, atlikite veiksmus, aprašytus skyriuje Slaptažodžių tvarkytuvo sinchronizavimo [trikčių šalinimas naudojant "Azure AD" Prisijungimas sinchronizavimą.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







