---
title: Problemos su kredencialais
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063681"
---
# <a name="issues-with-credentials"></a>Problemos su kredencialais

["Microsoft" tapatybės platforma ir "OAuth" 2,0 kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) aprašo, kaip programa tiesiogiai atitinka "oauth 2,0" kliento kredencialų suteikimo srautą.

**Kaip valdyti taikomosios programos slaptažodį arba sertifikato kredencialus?**

"Azure CLI" galite naudoti [AZ ad taikomosios programos](https://docs.microsoft.com/cli/azure/ad/app/credential) kredencialus, kad panaikintumėte, sąraše arba iš naujo nustatytumėte taikomosios programos slaptažodį arba sertifikato kredencialus.

**Kaip iš naujo nustatyti vartotojų slaptažodžius?**

Vartotojai turi [registruotis savitarnos slaptažodžio nustatymo iš naujo,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) kad galėtų iš naujo nustatyti savo slaptažodžius. Užregistravus vartotoją, jie gali vadovautis šiame straipsnyje pateiktomis instrukcijomis, kad iš naujo nustatytumėte slaptažodį: [darbo arba mokymo įstaigos slaptažodžio nustatymas iš naujo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Kaip mano vartotojai keičia savo slaptažodžius?**

Vartotojai gali atlikti šiame straipsnyje nurodytus veiksmus, kad pakeistų slaptažodžius: [kaip pakeisti slaptažodį](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Jie taip pat gali [valdyti taikomųjų programų slaptažodžius dviem veiksmais](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Mano vartotojas gauna klaidą keičiant arba iš naujo nustatant slaptažodį**

Šis saitas pateiks informaciją apie įprastas problemas, kurios gali iškilti, kai vartotojas bando iš naujo nustatyti slaptažodį: [Dažniausios problemos ir jų sprendimai](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Iškilo problema iš naujo nustatant vartotojo slaptažodį**

- Įsitikinkite, kad turite teisę iš naujo nustatyti slaptažodžius. *Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.* Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.

- Įsitikinkite, kad suprantate licencijavimo reikalavimus:

  - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje:
    - **Tik debesies vartotojai** – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"
    - **Debesies ir (arba) vietiniai vartotojai – "** Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)
    - Jei norite sužinoti daugiau apie licencijavimo reikalavimus, skaitykite " [AZURE AD" savitarnos slaptažodžio nustatymo iš naujo licencijavimo reikalavimus](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Norėdami iš naujo nustatyti vartotojo slaptažodį, raskite vartotoją "Azure AD". Po to vartotojo Apžvalgos disku spustelėkite mygtuką iš naujo nustatyti slaptažodį.

**Slaptažodžio nustatymo iš naujo mygtukas yra pilkas**

Jūs neturite teisę iš naujo nustatyti **šio** vartotojo slaptažodžių. *Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.* Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.

**Nematau slaptažodžio nustatymo iš naujo ašmenų**

Jūs nesate įgalioti iš naujo nustatyti slaptažodžius. *Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.* Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.

**Nematau vietinio integravimo peilio slaptažodžio nustatymo iš naujo**

- Vietinis integravimo peilis rodomas tik hibridinėse aplinkose – tai reiškia, kad naudojate slaptažodį write, kad galėtumėte manipuliuoti vietinio vartotojo slaptažodžiais.

- Nematote šio disko, jei:

  - Nenaudojate slaptažodžio įrašymo atgal
  - Iškilo problema dėl slaptažodžio įrašymo ir diegimo ryšio
  - Iškilo "Azure AD Connect" diegimo/ryšio problema
  - Jei reikia daugiau trikčių šalinimo veiksmų problemoms su slaptažodžiais write, žiūrėkite [slaptažodžio įrašymo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nežinau, kaip iš naujo nustatyti vartotojo slaptažodį**

1. Prisijunkite prie "Azure" portalo kaip tinkamo administratoriaus.
2. Eikite į diską **vartotojai ir grupės** , pasirinkite **visi vartotojai**.
3. Pasirinkite vartotoją iš sąrašo.
4. Pasirinktam vartotojui pasirinkite **apžvalga**, tada komandų juostoje pasirinkite **iš naujo nustatyti slaptažodį**.
5. Pasirinkite mygtuką **iš naujo nustatyti slaptažodį** ir vadovaukitės ekrane pateikiamomis instrukcijomis.
    - Tik iš naujo vykdomas " **Azure" portalo** palaikymo slaptažodžio įrašymo metu.

**Iš naujo nustatyti vietinio vartotojo slaptažodį iš "Office 365" administravimo portalo arba "Office 365 Mobile" taikomosios programos, tačiau vartotojas vis tiek negali prisijungti**

Slaptažodžio write-back nepalaiko šiame portale. Iš naujo nustatyti vartotojo slaptažodį dar kartą "Azure" portale.
