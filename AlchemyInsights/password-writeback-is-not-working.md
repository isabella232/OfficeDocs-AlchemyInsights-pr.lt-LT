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
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999752"
---
# <a name="password-writeback-is-not-working"></a>Neveikia slaptažodžio įrašymo atgalinis skambinimas

**Kyla problemų konfigūruojant slaptažodžio įrašymo atgalinio kopijavimo**

- Slaptažodžio nurašymas yra aukščiausios kokybės funkcija.
- Įsitikinkite, kad suprantate licencijavimo reikalavimus:
  - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje
  - **Tik debesies vartotojai** – bet Office 365 (O365) sumokėjo SKU arba "Azure AD Basic"
  - **Debesies ir (arba)** vietinės vartotojų – "Azure AD Premium P1 arba P2, Enterprise Mobility + Security (EMS) arba Secure Productive Enterprise (SPE)
    - Norėdami sužinoti daugiau apie licencijavimo reikalavimus, žr. ["Azure AD" savitarnos slaptažodžio nustatymo iš naujo licencijavimo reikalavimai](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Turite bent vieną administratoriaus paskyrą ir vieną bandomąją vartotojo paskyrą su viena iš atitinkamų licencijų.
- Turite prijungti "Azure AD Prisijungimas prie pirminio domeno valdiklio emuliatoriaus, kad veiktų slaptažodžio įrašymo atgalinis valdiklis. Galite konfigūruoti "Azure AD Prisijungimas naudoti pirminio domeno valdiklį  dešiniuoju pelės mygtuku spustelėdami "Active Directory" sinchronizavimo jungties **ypatybes, tada pasirinkdami konfigūruoti katalogų skaidinius.** Iš ten ieškokite domeno **valdiklio ryšio parametrų** skyriaus ir pažymėkite žymės langelį, pavadintą **Naudoti tik pageidaujamus domeno valdiklius.**
  > [!NOTE]
  > Jei pageidaujama DC nėra PDC emuliatorius, "Azure AD Prisijungimas vis tiek pasieks PDC slaptažodžio įrašymo atgalinę kopiją.
- Jūsų nuomotoje buvo sukonfigūruotas ir įgalintas slaptažodžio nustatymas iš naujo. Daugiau informacijos žr. [Vartotojų įgalinkite iš naujo nustatyti "Azure AD" slaptažodžius.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Įsitikinkite, kad administratoriaus paskyra, naudojama slaptažodžio "Writeback" įgalinimo funkciją, yra debesies administratoriaus paskyra (sukurta "Azure AD" ne vietiniame AD)
- Turite vieną arba kelių miškų AD vietinę įdiegtį, kuriame veikia "Windows Server 2008 R2", "Windows Server 2012" arba "Windows Server 2012 R2" su įdiegtais naujausiais pakeitimų paketais
- Turite įdiegtą "Azure AD Prisijungimas įrankį ir paruošėte AD aplinką sinchronizuoti su debesimi. Prieš išbandę slaptažodžio įrašymo atgalį, įsitikinkite, kad iš pradžių visiškai importuojate ir visiškai sinchronizuojate "Azure AD" ir "Azure AD" Prisijungimas.
- Norėdami sužinoti daugiau, žr., kaip atlikti visišką [sinchronizavimą ir visišką importavimą "Azure AD" Prisijungimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Kyla problemų dėl slaptažodžio įrašymo atgalinio skambinimo ryšio**

1. Naujausios ["Azure AD"](https://www.microsoft.com/download/details.aspx?id=47594) versijos atsisiuntimas ir Prisijungimas
2. Užkardos konfigūracija: "Azure AD Prisijungimas įrankis (1.1.443 ir aukščiau) reikės **siuntimo HTTPS** prieigos prie:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Leisti, kad laukimo būsenos ryšiai tęsis bent 2–3 minutes

**Vis dar kyla problemų dėl slaptažodžio įrašymo**

- Jei vis tiek kyla problemų, pabandykite išjungti ir iš naujo įgalinti slaptažodžio įrašymo paslaugą "Azure AD" Prisijungimas įrankį
- Norėdami sužinoti daugiau, žr., kaip išjungti [ir iš naujo įgalinti slaptažodžio įrašymo atgalinę jungtį](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
