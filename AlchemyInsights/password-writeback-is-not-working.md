---
title: Neveikia slaptažodžio įrašymo atgalinis skambinimas
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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324931"
---
# <a name="password-writeback-is-not-working"></a>Neveikia slaptažodžio įrašymo atgalinis skambinimas

**Kyla problemų konfigūruojant slaptažodžio įrašymo atgalinio kopijavimo**

- Slaptažodžio nurašymas yra aukščiausios kokybės funkcija.
- Įsitikinkite, kad suprantate licencijavimo reikalavimus:
  - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje
  - **Tik debesies vartotojai** – bet Office 365 (O365) mokami SKU arba "Azure AD Basic"
  - **Debesies ir (arba)** vietinį vartotojų – "Azure AD Premium P1 arba P2, Enterprise Mobility + Security (EMS) arba Secure Productive Enterprise (SPE)
    - Norėdami sužinoti daugiau apie licencijavimo reikalavimus, žr. ["Azure AD" savitarnos slaptažodžio nustatymo iš naujo licencijavimo reikalavimai](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Turite bent vieną administratoriaus paskyrą ir vieną bandomąją vartotojo paskyrą su viena iš atitinkamų licencijų.
- Turite prijungti "Azure AD Prisijungimas prie pirminio domeno valdiklio emuliatoriaus, kad veiktų slaptažodžio nurašymas. Galite konfigūruoti "Azure AD Prisijungimas naudoti pirminio domeno valdiklį  dešiniuoju pelės mygtuku spustelėdami "Active Directory" sinchronizavimo jungties **ypatybes, tada pasirinkdami konfigūruoti katalogų skaidinius.** Iš ten ieškokite domeno **valdiklio ryšio parametrų** skyriaus ir pažymėkite žymės langelį, pavadintą **naudoti tik pageidaujamus domeno valdiklius.**
    **Pastaba:Jei** pageidaujama DC nėra PDC emuliatorius, "Azure AD Prisijungimas vis tiek pasieks PDC slaptažodžio įrašymo atgalinę kopiją.
- Jūsų nuomotoje buvo sukonfigūruotas ir įgalintas slaptažodžio nustatymas iš naujo. Daugiau informacijos žr. [Vartotojų įgalinkite iš naujo nustatyti "Azure AD" slaptažodžius.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Įsitikinkite, kad administratoriaus paskyra, naudojama slaptažodžio "Writeback" įgalinimo funkciją, yra debesies administratoriaus paskyra (sukurta "Azure AD" ne vietiniame AD)
- Turite vieną arba kelių miškų AD vietinę įdiegtį, kuriame veikia "Windows Server 2008 R2", "Windows Server 2012" arba "Windows Server 2012 R2" su įdiegtais naujausiais pakeitimų paketais
- Turite įdiegtą "Azure AD Prisijungimas įrankį ir paruošėte AD aplinką sinchronizuoti su debesimi. Prieš išbandę slaptažodžio įrašymo atgalį, įsitikinkite, kad iš pradžių visiškai importuojate ir visiškai sinchronizuojate "Azure AD" ir "Azure AD" Prisijungimas.
- Norėdami sužinoti daugiau, sužinokite, kaip atlikti visišką [sinchronizavimą ir visišką importavimą "Azure AD" Prisijungimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Kyla problemų dėl slaptažodžio įrašymo atgalinio skambinimo ryšio**

1. Naujausios ["Azure AD"](https://www.microsoft.com/download/details.aspx?id=47594) versijos atsisiuntimas ir Prisijungimas
2. Užkardos konfigūracija: "Azure AD Prisijungimas įrankis (1.1.443 ir aukščiau) reikės **siuntimo HTTPS** prieigos prie:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Leisti, kad laukimo būsenos ryšiai tęsis bent 2–3 minutes

**Vis dar kyla problemų dėl slaptažodžio įrašymo atgalinio įrašymo**

- Jei vis tiek kyla problemų, pabandykite išjungti ir iš naujo įgalinti slaptažodžio įrašymo paslaugą "Azure AD Prisijungimas" įrankyje
- Norėdami sužinoti daugiau, žr., kaip išjungti [ir iš naujo įgalinti slaptažodžio įrašymo atgalinę jungtį](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
