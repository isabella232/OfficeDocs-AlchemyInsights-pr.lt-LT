---
title: Neveikia slaptažodis write
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243516"
---
# <a name="password-writeback-is-not-working"></a>Neveikia slaptažodis write

**Kilo problemų konfigūruojant slaptažodžius**

- Slaptažodis write-back yra priemoka funkcija.
- Įsitikinkite, kad suprantate licencijavimo reikalavimus:
  - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje
  - **Tik debesies vartotojai** – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"
  - **Debesies ir (arba) vietiniai vartotojai – "** Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)
    - Norėdami sužinoti daugiau apie licencijavimo reikalavimus, skaitykite " [AZURE AD" savitarnos slaptažodžio nustatymo iš naujo licencijavimo reikalavimai](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Turite bent vieną administratoriaus paskyrą ir vieną bandomosios vartotojo paskyrą su viena iš atitinkamos licencijos.
- Turite prijungti "Azure AD Connect" prie pirminio domeno valdiklio emuliatorius, kad veiktų slaptažodis. Galite sukonfigūruoti "Azure AD Connect" naudoti pirminį domeno valdiklį dešiniuoju pelės mygtuku spustelėdami "Active Directory" sinchronizavimo jungties **ypatybes** , tada pasirinkite **Konfigūruoti katalogų skaidinius**. Čia ieškokite skyriaus **domeno valdiklio ryšių parametrai** ir pažymėkite žymės langelį **naudoti tik pageidaujamus domenų valdiklius**.
  > [!NOTE]
  > Jei pageidaujamas DC nėra PDC emuliatorius, "Azure AD Connect" vis tiek pasieks slaptažodžių įrašymo PDC.
- Slaptažodžio nustatymas iš naujo sukonfigūruotas ir įgalintas jūsų nuomotojuje. Daugiau informacijos ieškokite [vartotojų įgalinimas iš naujo nustatyti "AZURE AD" slaptažodžius](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Įsitikinkite, kad administratoriaus abonementas, naudojamas slaptažodžiui write, yra debesies administratoriaus abonementas (sukurtas "Azure AD" ne vietiniame skelbime)
- Turite vieną arba kelių miškų skelbimą vietiniame diegime, kuriame veikia "Windows Server" 2008 R2, "Windows Server 2012" arba "Windows Server 2012 R2" su įdiegtais naujausiais pakeitimų paketais
- Įdiegtas "Azure AD Connect" įrankis ir jūs paruošėte skelbimo aplinką, skirtą sinchronizuoti debesyje. Prieš išbandydami slaptažodį write, įsitikinkite, kad pirmą kartą atliekate visą importavimą ir visišką sinchronizavimą iš AD ir Azure AD "Azure AD Connect".
- Norėdami sužinoti daugiau, Sužinokite, kaip atlikti [visas sinchronizavimo ir visas importavimas naudojant "AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations) "

**Iškilo problema dėl slaptažodžio įrašymo atgal ryšio**

1. Naujausios " [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594) " versijos atsisiuntimas ir įjungimas
2. Užkardos konfigūracija: "Azure AD Connect" įrankyje (1.1.443 ir anksčiau) reikės **siuntimo https** prieigos:
    - passwordreset.microsoftonline.com
    - servicebus. Windows. Networks
3. Leisti naudoti tuščiosios eigos ryšius bent 2-3 min.

**Vis dar kyla problemų dėl slaptažodžio įrašymo**

- Jei vis tiek kyla problemų, bandykite išjungti ir iš naujo įgalinti slaptažodžio įrašymo paslaugą "Azure AD Connect" įrankyje
- Norėdami sužinoti daugiau, Sužinokite, kaip [išjungti ir iš naujo įjungti slaptažodį write-back](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
