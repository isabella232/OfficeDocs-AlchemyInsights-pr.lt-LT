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
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019516"
---
# <a name="authentication-issues"></a>Autentifikavimo problemos

**Ieškote informacijos apie AADSTS klaidų kodus, kuriuos pateikia „Azure Active Directory“ („Azure AD“) saugos atpažinimo ženklų tarnyba (STS)?** Peržiūrėkite [„Azure AD“ autentifikavimo ir autorizavimo klaidų kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes), kad rastumėte AADSTS klaidų aprašus, taisymus ir kai kuriuos siūlomus sprendimus.

Autorizavimo klaidos gali atsirasti dėl kelių skirtingų problemų, kurių dauguma generuoja 401 arba 403 klaidą. Pavyzdžiui, autorizavimo klaidų gali kilti dėl šių problemų:

- Netinkami [atpažinimo ženklo gavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Prastai konfigūruotos [teisių aprėptys](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) trūkumas

Norėdami išspręsti dažniausiai pasitaikančių autorizavimo klaidų problemą, bandykite atlikti toliau nurodytus veiksmus, kurie labiausiai atitinka gaunamą klaidą. Gaunamai klaidai gali būti taikomas daugiau negu vienas žingsnis.

**401 neįgaliotos prieigos klaida: ar jūsų atpažinimo ženklas tinkamas?**

Įsitikinkite, kad programa kaip užklausos dalį pateikia tinkamą prieigos atpažinimo ženklą „Microsoft Graph“. Ši klaida dažnai reiškia, kad prieigos atpažinimo ženklo gali trūkti HTTP autentifikavimo užklausos antraštėje arba kad atpažinimo ženklas yra netinkamas ar baigėsi jo galiojimas. Primygtinai rekomenduojame naudoti „Microsoft“ autentifikavimo biblioteką (MSAL) prieigos atpažinimo ženklo gavimui. Be to, ši klaida gali įvykti, jei bandote naudoti įgaliotosios prieigos atpažinimo ženklą, suteiktą asmeninei „Microsoft“ paskyrai, kad pasiektumėte API, palaikančią tik darbo arba mokymo įstaigos paskyras (organizacijos paskyras).

**403 draudžiamos prieigos klaida: ar pasirinkote tinkamą teisių rinkinį?**

Įsitikinkite, kad pageidaujate tinkamo teisių rinkinio, pagrįsto programos „Microsoft Graph“ API. Rekomenduojamos mažiausiai privilegijuotos teisės yra pateiktos visose „Microsoft Graph“ API nuorodos metodų temose. Be to, šias teises programai turi suteikti vartotojas arba administratorius. Paprastai teisės suteikiamos sutikimo puslapyje arba naudojant „Azure Portal“ programos registracijos portalą. Programos dalyje **Parametrai** spustelėkite **Būtinos teisės**, tada spustelėkite **Suteikti teises**. Daugiau informacijos rasite:

- [„Microsoft Graph“ teisės](https://docs.microsoft.com/graph/permissions-reference) 
- [Apie „Azure AD“ teises ir sutikimą](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 draudžiamos prieigos klaida: ar programa gavo atpažinimo ženklą, kad atitiktų pasirinktas teises?**

Įsitikinkite, kad prašomų arba suteiktų teisių tipai atitinka programos gaunamo prieigos atpažinimo ženklo tipą. Gali būti, kad prašote ir suteikiate programos teises, tačiau naudojate įgaliotuosius interaktyviuosius kodo srauto atpažinimo ženklus vietoje kliento kredencialų srauto atpažinimo ženklų arba prašydami ir suteikdami įgaliotąsias teises, tačiau vietoje įgaliotųjų kodo srauto atpažinimo ženklų naudokite kliento kredencialų srauto atpažinimo ženklus.

Daugiau informacijos apie atpažinimo ženklų gavimą žr.:

- [Prieigos gavimas vartotojų ir įgaliotųjų teisių vardu](https://docs.microsoft.com/graph/auth-v2-user) 
- [„Azure AD“ v2.0 – „OAuth“ 2.0 autorizavimo kodo srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Prieigos gavimas nenaudojant vartotojo („daemon“ tarnyba) ir programos teisių](https://docs.microsoft.com/graph/auth-v2-service) 
- [„Azure AD v2.0 – „OAuth“ 2.0 kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 draudžiamos prieigos klaida: slaptažodžio nustatymas iš naujo**

Šiuo metu nėra jokių programos teisių, „daemon“ tarnybos tarnybai suteikimo teisių, kurios leistų nustatyti vartotojų slaptažodžius. Šios API palaikomos tik naudojant interaktyvių įgaliotųjų kodų srautus su prisiregistravusiu administratoriumi. Daugiau informacijos žr. [„Microsoft Graph“ teisės](https://docs.microsoft.com/graph/permissions-reference).

**403 draudžiama prieiga: ar vartotojas turi prieigą ir yra licencijuotas?**

Kai naudojamas įgaliotojo kodo srautas, „Microsoft Graph“ įvertina, ar užklausa buvo leidžiama pagal programai suteiktas teises ir prisijungusio vartotojo turimas teises. Paprastai ši klaida nurodo, kad vartotojui nepakanka teisių atlikti užklausą **arba** vartotojas neturi prieigos teisių prie duomenų. Užklausą sėkmingai gali pateikti tik vartotojai, kurie turi reikiamas teises arba licencijas.

**403 draudžiama prieiga: ar pasirenkate tinkamą išteklių API?**

API tarnybos, pvz., „Microsoft Graph“, patikrina, ar *aud* pareiškimas (auditorija) gautame prieigos atpažinimo ženkle atitinka reikšmę, kurios sau tikisi, jei taip nėra, įvyksta 403 draudžiamos prieigos klaida. Dažnai šį klaida gaunama bandant naudoti atpažinimo ženklą, gautą „Azure AD Graph“ API, „Outlook“ API arba „SharePoint“ / „OneDrive“ API, siekiant iškviesti „Microsoft Graph“ (arba atvirkščiai). Įsitikinkite, kad išteklius (arba aprėptis), kuriam programa gauna atpažinimo ženklą, atitinka API, kurią iškviečia programa.

**400 bloga užklausa arba 403 draudžiama prieiga: ar vartotojas atitinka organizacijos sąlyginės prieigos (CA) strategijas?**

Atsižvelgiant į organizacijos sąlyginės prieigos (CA) strategijas, vartotojui, kuris bando pasiekti „Microsoft Graph“ išteklius per programą, gali reikėti nurodyti papildomą informaciją, kurios nėra iš pradžių gautame prieigos atpažinimo ženkle. Tokiu atveju programa gauna **400 su *interaction_required*** klaidą bandant gauti prieigos atpažinimo ženklą, arba **403 su *insufficient_claims*** klaidą bandant iškviesti „Microsoft Graph“. Abiem atvejais klaidos atsakyme pateikiama papildomos informacijos, kurią galima pateikti įgaliotam pabaigos taškui, kad vartotojas galėtų pateikti papildomos informacijos (pvz., kelių dalių autentifikavimas arba įrenginio registracija).

Daugiau informacijos, susijusios su sąlygine prieiga, žr.:

- [Sąlyginės prieigos problemų sprendimas naudojant MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [„Azure Active Directory“ sąlyginės prieigos kūrėjų rekomendacijos](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***""Azure Active Directory"" autentifikavimo bibliotekos (ADAL) ir "Azure AD "Graph" API (AAD "Graph") palaikymo pabaiga***

- Nuo 2020 m. birželio 30 d. mes neįtrauksime jokių naujų funkcijų į „Azure Active Directory“ autentifikavimo biblioteką (ADAL) ir „Azure AD Graph“ API („AAD Graph“). Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.
- Nuo 2022 m. birželio 30 d. baigsime ADAL ir „AAD Graph“ palaikymą ir nebeteisime techninio palaikymo ar saugos naujinimų.
    - Programos, kurios naudoja ADAL esamoms OS versijoms, po šio laiko veiks ir toliau, tačiau negaus jokių techninio palaikymo ar saugos naujinimų.
    - P nurodytos datos programos, naudojančios „AAD Graph“, gali nebegauti atsakymų iš „AAD Graph“ galinio punkto.

**ADAL perkėlimas**

Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai. Ši rekomendacija pateikta kontekste, kai „Microsoft“ perkelia savo programas į MSAL iki palaikymo teikimo pabaigos. „Microsoft“ programų perkėlimo į MSAL tikslas yra užtikrinti, kad programos naudotų MSAL nuolatinius saugos ir funkcijų patobulinimus.

- [Skaityti ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Sužinokite, kaip perkelti programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jei reikia pagalbos norint suprasti, kurios iš programų naudoja ADAL, rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su nepriklausomais programinės įrangos teikėjais (ISV) ar programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Jei naudojate programas, kurios naudoja „AAD Graph“, vadovaukitės mūsų nurodymais, kaip [perkelti „Azure AD Graph“ programas į „Microsoft Graph“](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Mūsų perkėlimo kontroliniame sąraše apibūdinama darbo pradžia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali suteikti informacijos apie visą „AAD Graph“ naudojimą jūsų nuomotojuje.

 










