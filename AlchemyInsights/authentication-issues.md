---
title: Autentifikavimo problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974484"
---
# <a name="authentication-issues"></a>Autentifikavimo problemos

**Ieškote informacijos apie "AADSTS" klaidų kodus, kuriuos grąžino "Azure Active Directory" ("Azure AD") saugos atpažinimo ženklų tarnyba (STS)?** Peržiūrėkite " [AZURE AD" autentifikavimo ir autorizavimo klaidų kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , kad rastumėte AADSTS klaidų aprašus, pataisymus ir kai kuriuos siūlomus sprendimo būdus.

Autorizavimo klaidos gali kilti dėl kelių skirtingų problemų, kurių dauguma generuoja "401" arba "403" klaidą. Pvz., toliau nurodytos problemos gali sukelti autorizavimo klaidas:

- Neteisingi [prieigos žetono įsigijimo srautai](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Netinkamai sukonfigūruotos [teisių aprėptis](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) stoka

Norėdami išspręsti įprastas autorizavimo klaidas, išbandykite toliau pateiktus veiksmus, kurie labiausiai atitinka jūsų gaunamas klaidas. Dėl klaidos, kurią gaunate, gali būti taikomi daugiau nei vienas veiksmas.

- **401 Neleistina klaida: ar jūsų žetonas galioja?**

Įsitikinkite, kad jūsų programa pateikia tinkamą "Microsoft Graph" prieigos žetoną kaip užklausos dalį. Ši klaida dažnai reiškia, kad "Access" atpažinimo ženklas gali trūkti HTTP autentifikavimo užklausos antraštėje arba kad atpažinimo ženklas negalioja arba nebegalioja. Primygtinai rekomenduojame naudoti "Microsoft" autentifikavimo biblioteką (MSAL) "Access" atpažinimo ženklų įsigijimui. Be to, ši klaida gali įvykti, jei bandote naudoti įgaliotojo prieigos žetoną, suteiktą asmeniniam "Microsoft" abonementui, kad pasiektumėte API, kuris palaiko tik darbo arba mokymo įstaigos paskyras (organizacijos paskyras).

**403 Forbidden klaida: pasirinkote tinkamą teisių rinkinį?**

Įsitikinkite, kad prašėte tinkamo teisių rinkinio pagal "Microsoft Graph" API taikomųjų programų iškvietimus. Rekomenduojamos mažiausiai privilegijuotos teisės pateikiamos visose "Microsoft Graph" API nuorodų metodo temose. Be to, šios teisės turi būti suteiktos taikomajai programai pagal vartotoją arba administratorių. Teisių suteikimas paprastai įvyksta naudojant "Azure" portalo taikomosios programos registracijos peilio sutikimo puslapį arba naudojimą. Taikomosios programos **parametrų** ašmenys spustelėkite **reikiamas teises**, tada spustelėkite **suteikti teises**. Daugiau informacijos rasite:

- ["Microsoft Graph" teisės](https://docs.microsoft.com/graph/permissions-reference) 
- ["Azure AD" teisių ir sutikimo supratimas](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Forbidden klaida: ar jūsų programa įsigyja atpažinimo ženklą, kad atitiktų pasirinktas teises?**

Įsitikinkite, kad prašomos arba suteiktos teisės atitinka jūsų taikomosios programos "Access" atpažinimo ženklo tipą. Galite prašyti ir suteikti taikomųjų programų teises, bet naudoti interaktyvius interaktyviojo kodo srauto atpažinimo ženklus, o ne kliento kredencialų srauto atpažinimo ženklus, arba prašyti ir suteikti įgaliotasis teises, bet naudoti kliento kredencialų srauto atpažinimo ženklus vietoj įgaliotojo kodo srautų žetonų.

Daugiau informacijos, susijusios su žetonų įgijimui, rasite:

- [Gaukite prieigą vartotojų ir įgaliotų teisių vardu](https://docs.microsoft.com/graph/auth-v2-user) 
- ["Azure AD v 2.0" – "OAuth" 2,0 autorizavimo kodo srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Gaukite "Access" nenaudodami vartotojo (Daemon Service) ir taikomosios programos teisių](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0 kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 uždrausta klaida: slaptažodžio nustatymas iš naujo**

Šiuo metu nėra taikomųjų programų teisių demono paslaugų, kurios leidžia iš naujo nustatyti vartotojų slaptažodžius. Šios API palaikomos tik naudojant interaktyvius įgaliotojo kodo srautus su prisijungusiems administratoriui. Daugiau informacijos ieškokite ["Microsoft Graph" teisės](https://docs.microsoft.com/graph/permissions-reference).

**403 uždrausta: ar vartotojas turi prieigą ir jie yra licencijuoti?**

Jei tai yra įgaliotasis kodo srautai, "Microsoft Graph" įvertina, ar užklausa buvo suteikta remiantis programėlei suteiktomis teisėmis ir prisijungusiems vartotojui suteiktomis teisėmis. Paprastai ši klaida nurodo, kad vartotojas nėra pakankamai privilegijuotas, kad galėtų atlikti užklausą, **arba** vartotojas nėra licencijuotas duomenims, kurie yra pasiekiami. Užklausą gali sėkmingai atlikti tik vartotojai, turintys reikiamas teises arba licencijas.

**403 uždrausta: ar pasirinkote tinkamą išteklių API?**

API paslaugos, pvz., "Microsoft Graph", tikrina, kad "Access" atpažinimo ženklo *AUD* reikalavimas (auditorija) sutampa su jo paties nurodyta reikšme, o jei ne, įvyksta 403 uždrausta klaida. Dažna klaida dėl šios klaidos bando naudoti atpažinimo ženklą, įsigytą "Azure AD Graph" API, "Outlook" API arba "SharePoint"/"OneDrive" API, kad paskambintumėte į "Microsoft Graph" (arba atvirkščiai). Įsitikinkite, kad išteklių (arba aprėpties) jūsų programa įgyja atpažinimo ženklą, atitinkantį API, kurį skambina programa.

**400 netinkama užklausa arba 403 uždrausta: ar vartotojas laikosi savo organizacijos sąlyginės prieigos (CA) strategijų?**

Atsižvelgiant į organizacijos sąlyginės prieigos (CA) strategijas, vartotojui prieigą prie "Microsoft Graph" išteklių galima ginčyti naudojant papildomą informaciją, kuri nėra jūsų taikomosios programos "Access" atpažinimo ženkle. Šiuo atveju programa gauna **400 su *interaction_required*** klaida "Access" atpažinimo ženklų įsigijimo metu arba **403 su *Insufficient_claims*** klaida, kai skambinama į "Microsoft Graph". Abiem atvejais klaidos atsakyme yra papildomos informacijos, kurią galima pateikti įgaliotajam įverčiui, kad būtų galima užginčyti papildomą informaciją (pvz., kelių dalių autentifikavimą arba įrenginio registraciją).

Daugiau informacijos, susijusios su sąlygine prieiga, rasite:

- [Sąlyginės prieigos iššūkių naudojimas naudojant MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- ["Azure Active Directory" sąlyginės prieigos kūrėjo gairės](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

*" *_Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "AZURE ad Graph" API (AAD grafikas) palaikymo pabaiga_*

- Nuo birželio 30 d., 2020, nebegalėsime įtraukti jokių naujų funkcijų į "Azure Active Directory" autentifikavimo biblioteką (ADAL) ir "Azure AD Graph API" (AAD Graph). Mes ir toliau suteiksime techninio palaikymo ir saugos naujinimus, tačiau nebepateiksime funkcijų naujinimų.
- Nuo birželio 30 d., 2022, mes užbaigsime ADAL ir AAD Graph palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.
    - Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės gauti jokio techninio palaikymo ar saugos naujinimų.
    - Taikomosios programos, naudojančios AAD grafiką po šio laiko, gali nebegauti atsakymų iš AAD diagramos galinio punkto.

−*Adal perkėlimas**

Rekomenduojame naujinti į ["Microsoft" autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kuri turi naujausias funkcijas ir saugos naujinimus. Ši rekomendacija taikoma "Microsoft" perkeliant jos taikomąsias programas į MSAL pagal palaikymo pabaigos terminą. "Microsoft" programų perkėlimo į MSAL tikslas – užtikrinti, kad programos būtų naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.

- [DUK apie ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Sužinokite, kaip perkelti taikomąsias programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo nepriklausomu programinės įrangos pardavėjais (ISVs) arba taikomųjų programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti jums visų ne "Microsoft" ADAL taikomųjų programų sąrašą savo nuomotojuje.

**AAD Graph perkėlimas**

Jei naudojate "AAD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip [perkelti "AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- "Azure App" registracijos portale rodoma, kurios taikomosios programos naudoja AAD grafiką. Rekomenduojame Peržiūrėti visus savo taikomųjų programų šaltinio kodus ir, jei reikia, pasiekti bet kokius ISVs arba taikomųjų programų teikėjus. "Microsoft" palaikymas taip pat gali suteikti jums informaciją apie visus "AAD Graph" naudojimą savo nuomotojuje.

 










