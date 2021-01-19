---
title: Vartotojo trikčių šalinimas
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901042"
---
# <a name="announcements"></a>Skelbimai

Vadovaukitės "Google" rekomendacijomis dėl suderinamumo testavimo, kad patikrintumėte, ar jūsų taikomosios programos yra paveiktos. "Google" rekomendacijos pasiekiamos https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Įsitikinkite, kad prisijungiate prie savo vartotojų naudodami "Google" paskyras naudodami sistemos žiniatinklio rodinį arba sistemos naršyklę. Daugiau informacijos ieškokite straipsnyje [prisijungimo prie taikomosios programos (-ų) problemos naudojant tik "Chrome" naršyklę](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Negaliu sukurti naujo vartotojo "Azure AD" kataloge**

Kad išspręstumėte problemą, dėl kurios negalėsite sukurti naujo vartotojo "Azure AD", atlikite šiuos veiksmus:

1. Įsitikinkite, kad turite teisę sukurti naują standartinį vartotoją. Tik visuotinis administratorius arba vartotojo administratorius vaidmuo "Azure Active Directory" (AD) gali sukurti naują standartinį vartotoją. Jei nesate nė vieno iš šių vaidmenų, paprašykite administratoriaus, kad įtrauktumėte jus į vieną iš šių vaidmenų arba sukurtumėte naują vartotojo paskyrą.
2. Įsitikinkite, kad vartotojo vardas yra domene, kuris patikrintas jūsų "Azure AD". Jei "Azure AD" neturite jokių patikrintų pasirinktinio domenų vardų, galite naudoti "Azure AD" pradinį domeną, kuris baigiasi *. onmicrosoft.com.
3. Įsitikinkite, kad vartotojo vardas priklauso domenui, kuris nėra sujungtas su "Azure AD" iš vietinio skelbimo. Vartotojų negalima įtraukti į debesį su domenų pavadinimais, kurie yra susieti vietinėje organizacijoje.
4. Įsitikinkite, kad joks kitas vartotojas arba kontaktas jau turi vartotojo vardą, kurį norite priskirti naujam vartotojui. Vartotojų vardai turi būti unikalūs "Azure AD".
5. Ieškokite "Azure AD" [vaidmenų ir administratorių](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) "Azure AD".
6. Peržiūrėkite "Azure AD" [domenų vardus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) .
7. Peržiūrėkite [audito žurnalus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , kad matytumėte išsamesnę informaciją apie neseniai sukurtą arba panaikintą vartotoją, pvz., kas atliko veiksmą ir kada.
8. Daugiau informacijos apie naujų vartotojų įtraukimą ieškokite " [Azure" portalo naudojimas kuriant naują vartotoją "AZURE ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) ".
9. Daugiau informacijos apie administratoriaus vaidmenų teises "Azure AD" ieškokite " [AZURE AD" administravimo vaidmenys](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Informacijos, kaip kurti vartotoją naudojant "Azure AD PowerShell", ieškokite " [AZURE ad PowerShell", kad sukurtumėte naują vartotoją](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problema, susijusi su savitarnos registracija**

Norėdami šalinti problemas, susijusias su savitarnos registravimais, atlikite šiuos veiksmus:

1. Norėdami naudoti savitarnos prisijungimo naudodami taikomąsias programas, pirmiausia įjunkite savo nuomotojo savitarnos registravimosi paslaugą. 
2. Norėdami įgalinti taikomąją programą, skirtą naudoti savitarnos prisiregistruoti, įtraukite ją į savo vartotojo srautą. Kai kitąkart pereinate į tos taikomosios programos prisijungimo puslapį, matysite parinktį **_be paskyros? Sukurkite vieną!_* _. Taip pradedamas savitarnos prisijungimo procesas.
3. Informacijos, kaip naudoti savitarnos prisiregistruoti, kad būtų galima automatiškai įvesti organizaciją "Azure AD", ieškokite [savitarnos prisiregistruoti naudoti "AZURE ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)".
4. Susieję vartotojų srautą su viena ar daugiau taikomųjų programų, vartotojai, kurie lanko šią taikomąją programą, galės prisiregistruoti ir gauti svečio abonementą naudodami vartotojo sraute konfigūruotas parinktis. Daugiau informacijos apie svečio paskyros registraciją ir jos įgijimą vartotojai gali matyti [savitarnos registraciją Svečių vartotojams](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

*Problema kviečiant išorinį vartotoją**

Norėdami šalinti problemas, susijusias su kviečia išorinį vartotoją, atlikite toliau nurodytus veiksmus.

Įsitikinkite, kad siunčiate vartotojo kvietimą į elektroninio pašto adresą, atitinkantį vardą, su kuriuo vartotojas prisijungia. Jei siunčiate kvietimą į vartotojo tarpinio serverio pašto adresą, vartotojas negalės jo panaudoti. Daugiau informacijos ieškokite " [AZURE ad B2B" dokumentacijoje](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Negaliu priskirti licencijų vartotojui**

Norėdami šalinti triktis, susijusias su licencijų priskirimu vartotojui, atlikite šiuos veiksmus:

1. Norėdami valdyti vartotojų licencijas, įsitikinkite, kad naudojate abonementą su vienu iš būtinų administratoriaus vaidmenų: visuotinis administratorius, licencijos administratorius arba vartotojų administratorius. Galite patikrinti vartotojo vaidmenį skirtuke **katalogo vaidmuo** vartotojo ašmenimis.
2. Jei naudojate "Azure" portalą ir licencijų priskyrimas nepavyksta, spustelėkite pranešimą viršutiniame dešiniajame kampe. Atidaromas diskas su išsamia informacija apie tai, kas nutiko. Daugeliu atvejų užtenka suprasti ir išspręsti problemą.
3. Prieš vartotojui priskyrus licenciją, įsitikinkite, kad vartotojo ypatybė **naudojimo vieta** nustatyta. Patikrinkite, ar vartotojas turi tą ypatybę, peržiūrėdami vartotojo disko skirtuką **profilis** .
4. Įsitikinkite, kad yra pakankamai turimų produktų, kuriuos bandote priskirti, licencijų. Galite matyti galimų licencijų skaičių "Azure" portale, " [Azure Active Directory" > licencijos – > visus produktus](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Vartotojas jau gali turėti kitą licenciją, kurios tarnybos prieštarauja naujai licencijai, kurią bandote priskirti. Pavyzdžiui, jei vartotojas turi "Exchange Online" (1 plano) paslaugą, negalėsite priskirti licencijos "Exchange Online" (2 planas). Išjunkite vieną iš tarnybų, kad įgalintumėte naują licencijos paskyrimą. Jei naudojate "Azure" portalą arba "PowerShell" "cmdlet", **problemos išsamios informacijos** puslapyje išvardijamos konkrečios tarnybos, kurios sukelia konfliktą.
6. Jei bandote pašalinti licenciją ir nepavyksta, vartotojas gali turėti kitų licencijų su tarnybomis, priklausančiais nuo tarnybų, kurias bandote pašalinti. Jei naudojate "Azure" portalą arba "PowerShell" "cmdlet", klaidos pranešime bus išvardytos konkrečios tarnybos, turinčios priklausomybes.
7. Jei norite suprasti, kodėl buvo pridėta/pašalinta licencija (pvz., kas jūsų organizacijoje galėjo atlikti keitimai), patikrinkite audito žurnalus. Nustatykite filtrą su **licencijų veikla** , kad būtų rodomi visi pakeitimai, įskaitant "aktorius", kuris juos atliko.
8. Jei naudojate "Exchange Online", kai kurie jūsų nuomotojo vartotojai gali būti netinkamai sukonfigūruoti su ta pačia tarpinio serverio adreso reikšme. Tokiais atvejais galite matyti bendruosius klaidų pranešimą, kai licencijos operacija nepavyksta. [Šiame straipsnyje](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) pateikiama daugiau informacijos apie šią problemą, įskaitant informaciją apie tai, [kaip prisijungti prie "Exchange Online" naudojant nuotolinį "PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)". Norėdami nustatyti, kurie jūsų nuomotojo vartotojai turi tą patį tarpinio serverio adresą, vykdykite šią "Exchange Online" cmdlet:

Paleisti

Get-Recipient | kur yra {$ _. EmailAddresses – Match <user principal name> } | fL pavadinimas, RecipientType, emailaddresses





