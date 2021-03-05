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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482039"
---
# <a name="password-synchronization"></a>Slaptažodžių sinchronizavimas

**Slaptažodžių maišos sinchronizavimas neveiks**

Kai kurios Dažniausios problemos, su kuriomis susiduria Klientai, kai neveikia slaptažodžių maišos sinchronizavimas:

- "Azure AD Connect" naudojamos "Active Directory" paskyros ryšį su vietinio "Active Directory" nesuteiktas **lygiagretusis** katalogas ir **replikuoti katalogo pakeičiami visi** teisės, kurios reikalingos slaptažodžių sinchronizavimui – reikia tai pataisyti suteikiant šias teises "Active Directory" abonementui.
- Slaptažodžių maišos sinchronizavimas yra išjungtas, kai administratorius pakeitė vartotojo Sign-In metodą iš **Slaptažodžių sinchronizavimo** į kitą parinktį, pvz., **susiejimo su AD FS** "Azure AD Connect" vediklyje – galite tai pataisyti iš naujo įgalindami **slaptažodžių maišos sinchronizavimo** funkciją "Azure AD Connect" vediklyje.
- Ryšio problema su vietinio "Active Directory". Pvz., kai kurie domeno valdikliai nepasiekiami naudojant "Azure AD Connect" arba [būtini prievadai](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) yra blokuojami užkardos – reikia tai pataisyti užtikrindami, kad ryšys tarp "Azure AD Connect" serverio ir vietinio "Active Directory" veikia tinkamai.
- "Azure AD Connect" serveris šiuo metu yra sustojimo režimu, dėl kurio serveris negalės naudoti slaptažodžių, kad išspręstumėte problemą, atlikite veiksmus, aprašytus skyriuje " [AZURE AD Connect Sync" slaptažodžių Sinchronizavimo trikčių šalinimas – nesinchronizuojami jokie slaptažodžiai](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Slaptažodžių maišos sinchronizavimas neveikia kai kuriems vartotojams**

1. Jei pastebėjote, kad vartotojo slaptažodžio maiša nėra sinchronizuojamas, naudokite "Azure AD Connect" užduotį **Šalinti triktis** , kad sužinotumėte ir išspręstumėte problemą. Atlikite šias užduotis:

    a. [Paleiskite trikčių diagnostikos užduotį vediklyje](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Naudokite trikčių diagnostikos "cmdlet", kad ištirtumėte konkretaus naudojimo slaptažodžių maišos sinchronizavimo problemą](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Vietinis "Active Directory" vartotojo objektas įgalintas **vartotojui turi pasikeisti slaptažodį kitu registravimosi** parinktimi. Kai ši parinktis įgalinta, vartotojui priskiriamas laikinas slaptažodis ir būsite paraginti pakeisti slaptažodį kitame registravime. "Azure AD Connect" nesinchronizuoja laikinųjų slaptažodžių "Azure AD".

Norėdami išspręsti šią problemą, atlikite vieną iš šių užduočių:

- Paprašykite vartotojo prisijungti prie vietinio programos (pvz., "Windows" darbalaukio) ir pakeiskite slaptažodį. Naujasis slaptažodis bus sinchronizuojamas su "Azure AD".
- Administratorius turi atnaujinti vartotojo slaptažodį neįjungus parinkties **vartotojas turi pakeisti slaptažodį kitu prisijungimo metu** ir bendrinti naują slaptažodį su vartotoju.

3. Vietinio "Active Directory" vartotojo objektas **netinkamai sukonfigūruotas** objekto sinchronizacijai arba slaptažodžių sinchronizacijai. Norėdami pašalinti šią problemą, atlikite veiksmus, aprašytus skyriuje [slaptažodžių maišos Sinchronizavimo trikčių šalinimas naudojant "AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)".







