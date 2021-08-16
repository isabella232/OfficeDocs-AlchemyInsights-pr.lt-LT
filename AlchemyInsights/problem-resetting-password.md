---
title: Problema nustatant slaptažodį iš naujo
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039974"
---
# <a name="problems-resetting-password"></a>Slaptažodžio nustatymo iš naujo problemos

Toliau nurodytos kelios problemos, su kurias galite susidurti nustatydami slaptažodį iš naujo, ir galimi sprendimai:

**Kyla problemų dėl slaptažodžio nustatymo iš naujo, kuris netaikomas kitose kategorijose**

- Įsitikinkite, kad turite teisę iš naujo nustatyti slaptažodžius. Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius. Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratorių slaptažodžius.
- Įsitikinkite, kad suprantate licencijavimo reikalavimus:
    - Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje
        - Tik debesies vartotojai – bet Office 365 (O365) mokami SKU arba "Azure AD Basic"
        - Debesies ir (arba) vietinį vartotojų – "Azure AD Premium P1 arba P2, Enterprise Mobility + Security (EMS) arba Secure Productive Enterprise (SPE)
        - Norėdami daugiau sužinoti apie licencijavimo reikalavimus, žr. straipsnį "Azure AD" savitarnos [slaptažodžio nustatymo iš naujo licencijavimo reikalavimai.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kyla problemų bandant nustatyti slaptažodžio nustatymo iš naujo strategiją**

- Neseniai taikomos strategijos gali užtrukti kelias minutes, kad būtų galima pakartoti visuose duomenų centruose ir pabaigos taškuose. Fizinis atstumas nuo duomenų centro taip pat turės įtakos, kaip greitai taikomi keitimai.
- Patikrinkite, ar galutinis vartotojas, o ne administratorius, ir bandomasis su nedideliu vartotojų komplektu. Strategijos, sukonfigūruotos "Azure" portale ONLY, taikomos galutiniams vartotojams, o ne administratoriams. "Microsoft" užtikrina griežtą numatytąją "Azure" administratoriaus vaidmens dviejų vartų slaptažodžio nustatymo iš naujo strategiją (pvz., visuotinis administratorius, pagalbos tarnybos administratorius, slaptažodžių administratorius ir t. t.)
    - Sužinokite daugiau [apie administratoriams skirtas strategijas.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Noriu įdiegti slaptažodį iš naujo, bet nenoriu, kad mano vartotojai užregistruos papildomą saugos informaciją**

Iš anksto užpildykite vartotojų duomenis, kad jie jų neprisiims! - Jei esate administratorius, galite nustatyti vartotojų telefono ir el. pašto ypatybes prieš iš naujo nustatyti slaptažodį organizacijoje. Tai galite padaryti naudodami API, "PowerShell" arba "Azure AD" Prisijungimas. Daugiau informacijos čia:
- [Slaptažodžio nustatymo iš naujo diegimas nereikalaujant vartotojų registruotis](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Kokie duomenys naudojami iš naujo nustačius slaptažodį](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Slaptažodžio nustatymo iš naujo mygtukas yra pilkas**

Jums neleidžiama iš naujo nustatyti šio vartotojo slaptažodžių. Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius. Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratorių slaptažodžius.

**Nematau slaptažodžio nustatymo iš naujo ašmenų**

Jums neleidžiama iš naujo nustatyti slaptažodžių. Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius. Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratorių slaptažodžius.

**Slaptažodžio nustatymo iš naujo metu nematau vietinio integravimo disko**

- Vietinės integracijos ašmenys rodomas tik hibridinėse aplinkose, t. y. naudojate slaptažodžio nurašymo funkciją, kad valdysite vietinio vartotojo slaptažodžius.
- Nematote šio disko, jei:
    - Nenaudojate slaptažodžio įrašymo atgalinio
    - Kilo problemų dėl slaptažodžio įrašymo įrenginio / ryšio
    - Kilo "Azure AD" diegimo / ryšio Prisijungimas
    - Daugiau trikčių šalinimo veiksmų, susijusių su slaptažodžio įrašymo atgalinio rašymo trikčių šalinimu, žr. skyrių Slaptažodžio [įrašymo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nežinau, kaip iš naujo nustatyti vartotojo slaptažodį**

1. Prisijunkite prie "Azure" portalo kaip atitinkamas administratorius.
1. Eikite į vartotojų ir grupių ašmenį, pasirinkite **Visi vartotojai**.
1. Pasirinkite vartotoją iš sąrašo.
1. Pasirinktam vartotojui pasirinkite **Apžvalga**, tada komandų juostoje spustelėkite Iš naujo **nustatyti slaptažodį**.
1. Vykdykite ekrane pateiktas instrukcijas.
    - Iš naujo nustato tik "Azure" portalo palaikymo slaptažodžio įrašymo atgalinę kopiją.

**Iš naujo nustatou vietinio vartotojo slaptažodį iš "Office 365 Admin" portalo arba "Office 365 mobiliųjų įrenginių taikomosios programos, tačiau vartotojas vis tiek negali prisijungti**

Slaptažodžio rašymas šiame portale nepalaikomas. Iš naujo nustatykite vartotojo slaptažodį "Azure" portale – portal.azure.com

