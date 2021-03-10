---
title: Problemos nustatymo iš naujo slaptažodis
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696284"
---
# <a name="problems-resetting-password"></a>Problemos iš naujo nustatyti slaptažodį

Toliau pateikiami keli klausimai, su kuriais galite susidurti iš naujo nustatę slaptažodį ir galimus sprendimo būdus:

**Iškilo problema dėl slaptažodžio nustatymo iš naujo, neįtrauktos į kitas kategorijas**

- Įsitikinkite, kad turite teisę iš naujo nustatyti slaptažodžius. Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius. Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.
- Įsitikinkite, kad suprantate licencijavimo reikalavimus:
    - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje
        - Tik debesies vartotojai – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"
        - Debesies ir (arba) vietiniai vartotojai – "Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)
        - Norėdami sužinoti daugiau apie licencijavimo reikalavimus, peržiūrėkite straipsnį [licencijavimo reikalavimai, skirti "AZURE AD" savitarnos slaptažodžio nustatymo iš naujo](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Kilo problemų tikrinant slaptažodžio nustatymo iš naujo strategiją, kurią nustatėte**

- Neseniai taikytos strategijos gali užtrukti kelias minutes, kad būtų galima replikuoti visus duomenų centrus ir galutinius taškus. Fiziniai atstumai iš duomenų centro taip pat turės įtakos, kaip greitai keičiami keitimai.
- Išbandykite su galutinio vartotojo, o ne administratoriumi ir pilotu su nedideliu vartotojų rinkiniu. Strategijos, sukonfigūruotos "Azure" portale, taikomos tik galutiniams vartotojams, o ne administratoriams. "Microsoft" užtikrina, kad "Azure" administratoriaus vaidmuo būtų stipri numatytoji dviejų vartų slaptažodžio nustatymo iš naujo strategija (pvz.: visuotinis administratorius, pagalbos administratorius, slaptažodžių administratorius ir kt.)
    - Sužinokite daugiau apie [administratorių strategijas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Noriu įdiegti slaptažodį iš naujo, bet nenoriu, kad mano vartotojai užregistruotų papildomą saugos informaciją**

Iš anksto užpildyti jūsų vartotojų duomenis, kad jie neturėtų! -Kaip administratorius galite nustatyti savo vartotojams telefono ir elektroninio pašto ypatybes prieš atkurdami slaptažodį iš naujo savo organizacijai. Tai galite padaryti naudodami API, "PowerShell" arba "Azure AD Connect". Daugiau informacijos rasite čia:
- [Slaptažodžio nustatymo iš naujo diegimas nereikalaujant vartotojų registruotis](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Kokius duomenis naudoja slaptažodžio nustatymas iš naujo](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Slaptažodžio nustatymo iš naujo mygtukas yra pilkas**

Jūs neturite teisę iš naujo nustatyti šio vartotojo slaptažodžių. Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius. Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.

**Nematau slaptažodžio nustatymo iš naujo ašmenų**

Jūs nesate įgalioti iš naujo nustatyti slaptažodžius. Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius. Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.

**Nematau vietinio integravimo peilio slaptažodžio nustatymo iš naujo**

- Vietinis integravimo peilis rodomas tik hibridinėse aplinkose – tai reiškia, kad naudojate slaptažodį write, kad galėtumėte manipuliuoti vietinio vartotojo slaptažodžiais.
- Nematote šio disko, jei:
    - Nenaudojate slaptažodžio įrašymo atgal
    - Iškilo problema dėl slaptažodžio įrašymo ir diegimo ryšio
    - Iškilo "Azure AD Connect" diegimo/ryšio problema
    - Jei reikia daugiau trikčių šalinimo veiksmų problemoms su slaptažodžiais write, žr skyriuje [slaptažodžio įrašymo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nežinau, kaip iš naujo nustatyti vartotojo slaptažodį**

1. Prisijunkite prie "Azure" portalo kaip tinkamo administratoriaus.
1. Eikite į diską vartotojai ir grupės, pasirinkite **visi vartotojai**.
1. Pasirinkite vartotoją iš sąrašo.
1. Pasirinktam vartotojui pasirinkite **apžvalga**, tada komandų juostoje spustelėkite **iš naujo nustatyti slaptažodį**.
1. Vadovaukitės ekrane pateikiamomis instrukcijomis.
    - Tik iš naujo vykdomas "Azure" portalo palaikymo slaptažodžio įrašymo metu.

**Iš naujo nustatyti vietinio vartotojo slaptažodį iš "Office 365" administravimo portalo arba "Office 365 Mobile" taikomosios programos, tačiau vartotojas vis tiek negali prisijungti**

Slaptažodžio write-back nepalaiko šiame portale. Iš naujo nustatyti vartotojo slaptažodį dar kartą "Azure" portale – portal.azure.com

