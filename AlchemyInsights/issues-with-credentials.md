---
title: Kredencialų problemos
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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986827"
---
# <a name="issues-with-credentials"></a>Kredencialų problemos

"Microsoft" tapatybės platforma ir ["OAuth 2.0" kliento](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) kredencialų srautas aprašo, kaip programuoti tiesiogiai pagal "OAuth 2.0" kliento kredencialų teikimo srautą.

**Kaip valdyti programos slaptažodį arba sertifikato kredencialus?**

"Azure CLI" galite naudoti ["az" reklamos](https://docs.microsoft.com/cli/azure/ad/app/credential) programos kredencialus, kad panaikinsite, siųsite arba iš naujo nustatysite programos slaptažodį arba sertifikato kredencialus.

**Kaip mano vartotojai iš naujo nustato savo slaptažodžius?**

Vartotojai turi [registruotis, kad galėtų iš naujo nustatyti savo](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) slaptažodžius, kad galėtų nustatyti savitarnos slaptažodį iš naujo. Užregistravęs vartotoją, jis gali vadovautis šiame straipsnyje pateiktomis instrukcijomis ir iš naujo nustatyti slaptažodį: [Iš naujo nustatyti darbo arba mokymo įstaigos slaptažodį.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kaip mano vartotojai keičia savo slaptažodžius?**

Vartotojai gali atlikti šiame straipsnyje nurodytus veiksmus, kad pakeistų savo slaptažodžius: [Kaip pakeisti slaptažodį](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Jie taip pat [gali valdyti programų slaptažodžius, kad būtų galima patvirtinti dviem veiksmais.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mano vartotojas gauna klaidą keisdamas arba iš naujo nustatydamas savo slaptažodį**

Šis saitas pateiks informacijos apie įprastas problemas, kurios gali kilti vartotojui bandant iš naujo nustatyti slaptažodį: [dažnai pasitaikančių problemų ir jų sprendimų](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Kyla problemų nustatant vartotojo slaptažodį iš naujo**

- Įsitikinkite, kad turite teisę iš naujo nustatyti slaptažodžius. *Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.* Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratorių slaptažodžius.

- Įsitikinkite, kad suprantate licencijavimo reikalavimus:

  - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje:
    - **Tik debesies vartotojai** – bet Office 365 (O365) sumokėjo SKU arba "Azure AD Basic"
    - **Debesies ir (arba)** vietinės vartotojų – "Azure AD Premium P1 arba P2, Enterprise Mobility + Security (EMS) arba Secure Productive Enterprise (SPE)
    - Norėdami sužinoti daugiau apie licencijavimo reikalavimus, žr. "Azure AD" savitarnos [slaptažodžio nustatymo iš naujo licencijavimo reikalavimai.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Norėdami iš naujo nustatyti vartotojo slaptažodį, raskite vartotoją "Azure AD". Tada to vartotojo apžvalgos ašmenyje spustelėkite mygtuką Nustatyti slaptažodį iš naujo.

**Slaptažodžio nustatymo iš naujo mygtukas yra pilkas**

Jums neleidžiama iš naujo **nustatyti** šio vartotojo slaptažodžių. *Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.* Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratorių slaptažodžius.

**Nematau slaptažodžio nustatymo iš naujo ašmenų**

Jums neleidžiama iš naujo nustatyti slaptažodžių. *Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.* Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratorių slaptažodžius.

**Slaptažodžio nustatymo iš naujo metu nematau vietinio integravimo disko**

- Vietinės integracijos ašmenys rodomas tik hibridinėse aplinkose, t. y. naudojate slaptažodžio nurašymo funkciją, kad valdysite vietinio vartotojo slaptažodžius.

- Nematote šio disko, jei:

  - Nenaudojate slaptažodžio įrašymo atgalinio
  - Kilo problemų dėl slaptažodžio įrašymo įrenginio / ryšio
  - Kilo "Azure AD" diegimo / ryšio Prisijungimas
  - Daugiau trikčių šalinimo veiksmų, susijusių su slaptažodžio įrašymo atgal, žr. Slaptažodžio [įrašymo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nežinau, kaip iš naujo nustatyti vartotojo slaptažodį**

1. Prisijunkite prie "Azure" portalo kaip atitinkamas administratorius.
2. Eikite į **vartotojų ir grupių ašmenį,** pasirinkite Visi **vartotojai**.
3. Pasirinkite vartotoją iš sąrašo.
4. Pasirinktam vartotojui pasirinkite **Apžvalga**, tada komandų juostoje pasirinkite Iš naujo **nustatyti slaptažodį**.
5. Pasirinkite mygtuką **Iš naujo nustatyti** slaptažodį ir vykdykite ekrane pateiktas instrukcijas.
    - Iš naujo nustato tik **"Azure" portalo palaikymo** slaptažodžio įrašymo atgalinę kopiją.

**Iš naujo nustatou vietinio vartotojo slaptažodį iš "Office 365 Admin" portalo arba "Office 365 mobiliųjų įrenginių taikomosios programos, tačiau vartotojas vis tiek negali prisijungti**

Slaptažodžio rašymas šiame portale nepalaikomas. Iš naujo nustatykite vartotojo slaptažodį "Azure" portale.
