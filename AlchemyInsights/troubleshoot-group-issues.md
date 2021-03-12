---
title: Grupės problemų šalinimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714052"
---
# <a name="troubleshoot-group-issues"></a>Grupės problemų šalinimas

**Man reikia priskirti grupę "Azure AD" vaidmeniui**

Norėdami priskirti "Azure Active Directory" (AD) grupę "Azure AD" vaidmeniui, atlikite šiuos veiksmus:

1. Kurti naują grupę – kurti naują grupę:

    a. Prisijunkite prie "Azure AD" administravimo centro su privilegijuotu vaidmenų administratoriumi arba visuotinio administratoriaus teisėmis. 
    b. Pasirinkite "Azure Active Directory" > grupės > visos grupės > nauja grupė. 
    c. Kurti grupę.

2. Priskirti grupės vaidmenį grupės kūrimo metu arba sukūrus grupę.

    a. Norėdami priskirti grupės vaidmenį grupės kūrimo metu, įjunkite "Azure AD" vaidmenis, kuriuos galima priskirti grupei ir kurti grupę.
    b. Norėdami priskirti vaidmenį grupei po to, kai jis buvo sukurtas, pereikite į naujai sukurtos grupės skirtuką priskirti vaidmenys ir priskirkite grupei vaidmenį.

**Man reikia valdyti grupės, priskirtos "Azure AD" vaidmeniui, narystę**

1. Norint išvengti teisių didesnių teisių, pagal numatytuosius numatytuosius, tik privilegijuotas vaidmenų administratorius ir visuotinis administratorius gali modifikuoti vaidmeniui priskirtos grupės narystę. Tačiau jie gali pasirinkti priskirti tokiai grupei savininką ir pavesti šiai užduočiai. Daugiau informacijos rasite [naudodami debesies grupes, kad valdytumėte vaidmenų priskyrimus "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)".
2. Bendrųjų klausimų ir trikčių šalinimo patarimų, kaip priskirti vaidmenis "Azure AD" grupėms, ieškokite [trikčių šalinimo vaidmenys, priskirti debesies grupėms](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dinaminės grupės**

1. Jei negalite surasti įtaisytųjų vartotojo atributų, įsitikinkite, kad atributas yra palaikomų ypatybių sąraše.
2. Jei ieškote įtaisytųjų įrenginio atributų, įsitikinkite, kad atributas yra įrenginio atributų sąraše 
3. Be įtaisytojo vartotojo ir įrenginio atributų, taip pat galite naudoti [plėtinio atributus](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Sinchronizavus plėtinių atributus iš vietinio "Windows Server" arba prijungtos "SaaS" taikomosios programos, atributai turėtų būti matomi išplečiamame taisyklių kūrėjo sąraše. Pasirinktinio atributo pavadinimą galima rasti kataloge užklausant vartotojo atributo naudojant "PowerShell" ir ieškant atributo pavadinimo. Jie taip pat gali būti naudojami kuriant taisykles taisyklės sintaksėje.
4. Įsitikinkite, kad Jūsų Nuomotojas turi tinkamą licenciją. Dinamiškoms grupėms reikia, kad nuomininkas turėtų "Azure AD P1 Premium" licenciją. [Čia](https://azure.microsoft.com/pricing/details/active-directory/)galima rasti "Azure AD" licencijos planų sąrašą. [Čia](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)galima rasti įmonės mobilumo + saugos licencijavimo planus.
5. Įsitikinkite, kad vartotojo vaidmuo kuriant dinamišką grupę yra visuotinis administratorius, Intune administratorius, grupės administratorius arba vartotojo administratorius.
6. Leiskite grupei įvesti laiką. Atsižvelgiant į jūsų nuomotojo dydį, grupė gali užtrukti iki 24 valandų, kol ji bus pirmą kartą arba po taisyklės keitimo.
7. Daugiau informacijos ieškokite [pagal atributą pagrįstų taisyklių, skirtų dinaminės grupės narystei, kūrimas](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Reikia panaikinti grupę**

1. Grupes galima naikinti iš katalogo naudojant Remove-AzureADGroup cmdlet "Azure AD PowerShell" modulyje.
2. Prieš bandydami panaikinti sinchronizuotą grupę "Azure AD", įsitikinkite, kad panaikinote visas priskirtas licencijas, kad išvengtumėte klaidų.
3. Daugiau informacijos apie grupių naikinimą ieškokite [grupės naikinimas su priskirta licencija](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Reikia atkurti panaikintą grupę**

1. Jei "Office 365" grupė panaikinama, ją galima atkurti tik iki 30 dienų, kol bus panaikintas nuolatinis naikinimas. Panaikinus visam laikui, grupės nebebus galima atkurti. Sužinokite daugiau apie grupių atkūrimą [čia](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Ši funkcija nepalaikoma saugos grupių ir siuntimo grupių.
3. Įsitikinkite, kad turite teisę atkurti "Office 365" grupę. Visuotiniai administratoriai, grupės Administratoriai, vartotojų abonementų administratoriai, Intune tarnybų administratoriai, partnerio tier1 arba tier2 palaikymas ir grupės savininkas gali atkurti grupę.
4. Kai dinamiška grupė panaikinama ir atkuriama, ji vertinama kaip nauja grupė ir iš naujo įvedama pagal taisyklę. Šis procesas gali užtrukti iki 24 valandų.
5. Daugiau informacijos apie panaikintos grupės atkūrimą ieškokite [panaikinto "Office 365" grupės atkūrimas "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)".

**Grupės galiojimo strategijos konfigūracija**

1. Ši funkcija palaikoma tik "Office 365" grupėse, o ne saugos grupių ir paskirstymo grupių nepalaikomos.
2. Konfigūruojant ir naudojant "Office 365" grupių galiojimo strategiją reikia "Azure AD Premium" licencijos.
3. Šiuo metu "Office 365" grupių nuomotojuje galima sukonfigūruoti tik vieną galiojimo pabaigos strategiją.
4. Grupę gali atnaujinti tik visuotiniai administratoriai, grupės Administratoriai, vartotojų administratoriai ir grupės savininkas.
5. Jei "Office 365" grupės galiojimo laikas baigėsi, ji panaikinama ir gali būti atkurta tik iki 30 dienų, kol bus panaikintas nuolatinis naikinimas. Panaikinus visam laikui, grupės nebebus galima atkurti. Sužinokite daugiau apie grupių atkūrimą [čia](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Veikla pagrįstas Automatinis atnaujinimas**

"SharePoint", "Outlook" ir "teams" vartotojų veikla gali suaktyvinti grupės automatinį atnaujinimą. Veikla tikrinama 35 dienų prieš pasibaigiant grupės galiojimui. Jei dabartinio grupės gyvavimo laikotarpiu veikia veikla, grupė bus automatiškai atnaujinama, o elektroninio pašto pranešimas nebus siunčiamas grupės savininkams.

**Pasibaigusių grupių pranešimo laikas**

1. El. pašto pranešimai siunčiami "Office" 365 grupės savininkams 30 dienų, 15 dienų ir likus 1 dienai iki grupės galiojimo pabaigos.
2. Pirmą kartą nustačius galiojimo laiką, visos grupės, kurios yra senesnės nei galiojimo intervalas, nustatyta į "35" dienas iki galiojimo pabaigos.
3. Grupės galiojimo data skaičiuojama pagal grupės atnaujinimo datą, o ne pagal atnaujintą strategijos datą. Jei atnaujinama galiojimo pabaigos strategija, galiojimo pabaigos data nebus pakeista.
4. Daugiau informacijos rasite [grupės galiojimo strategijos ir atnaujinimo laiškų atnaujinimas](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) ir [atkūrimas panaikintą "Office 365" grupę "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Grupės kūrimo teisė**

Įsitikinkite, kad esate įgalioti kurti naują grupę. Visuotinis administratorius gali išjungti grupės kūrimą "Azure" portale arba "Access" skyde. Jums gali reikėti administratoriaus, kad galėtumėte sukurti jums naują grupę arba suteikti reikiamas teises.

1. [Naujos grupės kūrimas ir narių įtraukimas į "Azure" portalą](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Grupių kūrimas "PowerShell" MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Grupių kūrimo išjungimas "PowerShell"](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Valdyti, kas gali kurti grupes "Office 365"](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. ["Office 365" sutikimo pranešimo išjungimas naudojant "PowerShell"](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. ["Azure AD" administravimo vaidmenys](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Grupių kūrimo teisių valdymas**

1. Visuotiniai administratoriai gali valdyti saugos arba "Office 365" grupių kūrimo teises, sukurtas "Azure" portale arba "Access" skyde, nustatydami, kad **vartotojai gali kurti saugos grupes "Azure" portaluose** , o **vartotojai gali kurti "Office 365" grupes "Azure" portaluose** visose **grupėse > bendra (parametrai)**.
2. Taip pat galite apriboti grupės kūrimą, kad pasirinktumėte grupę vartotojų, jei turite "Azure AD P1 Premium" licenciją.

**Pasveikinimo pranešimo išjungimas naujiems "Office 365" grupės nariams**

Į "Office 365" grupes įtraukti vartotojai gali būti išjungti, kai "PowerShell" nustato reikšmę `UnifiedGroupWelcomeMessageEnabled` **klaidingai** . Sužinokite apie šį parametrą [čia](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













