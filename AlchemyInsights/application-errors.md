---
title: Taikomosios programos klaidos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931457"
---
# <a name="application-errors"></a>Taikomosios programos klaidos

Ieškote informacijos apie **AADSTS** klaidų kodus, kurie pateikiami iš ""Azure Active Directory" ("Azure AD") saugos atpažinimo ženklo tarnybos (STS)? Perskaitykite ["Azure AD" autentifikavimo](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) ir autorizavimo klaidų kodus, kad rastumėte AADSTS klaidų aprašus, pataisas ir kai kuriuos siūlomus sprendimo būdai.

Autorizavimo klaidos gali atsirasti dėl kelių skirtingų problemų, kurių dauguma generuoja 401 arba 403 klaidą. Pvz., dėl šių veiksmų gali kilti autorizavimo klaidų:

- Netinkami [atpažinimo ženklo gavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Prastai konfigūruotos [teisių aprėptys](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkumas

Norėdami išspręsti dažnai pasitaikančių autorizavimo klaidų problemą, pabandykite atlikti toliau nurodytus veiksmus, kurie labiausiai atitinka gaunamos klaidos rezultatus. Gali būti taikoma daugiau nei viena.

**401 neįgaliotos prieigos klaida: ar jūsų atpažinimo ženklas tinkamas?**

Įsitikinkite, kad jūsų taikomoji programa pateikia galiojantį prieigos atpažinimo ženklą "Microsoft "Graph" kaip užklausos dalį. Ši klaida dažnai reiškia, kad prieigos atpažinimo ženklo gali trūkti HTTP autentifikavimo užklausos antraštėje arba kad atpažinimo ženklas yra netinkamas ar baigėsi jo galiojimas. Primygtinai rekomenduojame naudoti ["Microsoft" autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) prieigos atpažinimo ženklų įsigijimui. Be to, ši klaida gali įvykti, jei bandote naudoti įgaliotosios prieigos atpažinimo ženklą, suteiktą asmeninei "Microsoft" paskyrai, norėdami pasiekti API, palaikančią tik darbo arba mokymo įstaigos paskyras (organizacijos paskyras).

**403 draudžiamos prieigos klaida: ar pasirinkote tinkamą teisių rinkinį?**

Patikrinkite, ar paprašėte tinkamo teisių rinkinio pagal "Microsoft "Graph" API, kuriuos skambinate programa. Rekomenduojamos mažiausiai privilegijuotos teisės teikiamos visose "Microsoft "Graph" API nuorodų metodo temose. Be to, šias teises programai turi suteikti vartotojas arba administratorius. Paprastai teisių suteikimas vyksta sutikimo puslapyje arba suteikiant teises naudojant "Azure Portal" taikomosios programos registracijos ašmenį. Programos dalyje **Parametrai** spustelėkite **Būtinos teisės**, tada spustelėkite **Suteikti teises**.

- [„Microsoft Graph“ teisės](https://docs.microsoft.com/graph/permissions-reference) 
- [Apie „Azure AD“ teises ir sutikimą](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 draudžiamos prieigos klaida: ar programa gavo atpažinimo ženklą, kad atitiktų pasirinktas teises?**

Įsitikinkite, kad pageidaujamos arba suteiktos teisės atitinka prieigos atpažinimo ženklo, kurį įsigyja jūsų programa, tipą. Galbūt prašote ir suteikiate taikomosios programos teises, tačiau vietoj kliento kredencialų srauto atpažinimo ženklų naudojate įgaliotuosius interaktyviuosius kodų srauto atpažinimo ženklus arba prašote ir suteikiate įgaliotąsias teises, tačiau vietoj įgaliotųjų kodų srauto atpažinimo ženklų naudokite kliento kredencialų srauto atpažinimo ženklus.

- [Prieigos gavimas vartotojų ir įgaliotųjų teisių vardu](https://docs.microsoft.com/graph/auth_v2_user) 
- [„Azure AD“ v2.0 – „OAuth“ 2.0 autorizavimo kodo srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Prieigos gavimas nenaudojant vartotojo („daemon“ tarnyba) ir programos teisių](https://docs.microsoft.com/graph/auth_v2_service) 
- [„Azure AD v2.0 – „OAuth“ 2.0 kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 draudžiamos prieigos klaida: slaptažodžio nustatymas iš naujo**

Šiuo metu nėra jokių programos teisių, „daemon“ tarnybos tarnybai suteikimo teisių, kurios leistų nustatyti vartotojų slaptažodžius. Šios API palaikomos tik naudojant interaktyvių įgaliotųjų kodų srautus su prisiregistravusiu administratoriumi.

- [„Microsoft Graph“ teisės](https://docs.microsoft.com/graph/permissions-reference)

**403 draudžiama prieiga: ar vartotojas turi prieigą ir yra licencijuotas?**

Naudojant įgaliotojo kodo srautus, "Microsoft "Graph"" įvertina, ar užklausa leidžiama atsižvelgiant į programai suteiktas teises ir teises, kurias turi prisijungęs vartotojas. Paprastai ši klaida nurodo, kad vartotojui nepakanka teisių atlikti užklausą arba vartotojas neturi prieigos teisių prie duomenų. Užklausą sėkmingai gali pateikti tik vartotojai, kurie turi reikiamas teises arba licencijas.

**403 draudžiama prieiga: ar pasirenkate tinkamą išteklių API?**

API tarnybos, pvz., "Microsoft "Graph"", patikrina, ar gautas prieigos atpažinimo ženklo aud reikalavimas (auditorija) atitinka reikšmę, kurios tikisi pats, o jei ne, įvyksta 403 Uždrausta klaida. Dažnai šį klaida gaunama bandant naudoti atpažinimo ženklą, gautą „Azure AD Graph“ API, „Outlook“ API arba „SharePoint“ / „OneDrive“ API, siekiant iškviesti „Microsoft Graph“ (arba atvirkščiai). Įsitikinkite, kad išteklius (arba aprėptis), kuriam programa gauna atpažinimo ženklą, atitinka API, kurią iškviečia programa.

**400 bloga užklausa arba 403 draudžiama prieiga: ar vartotojas atitinka organizacijos sąlyginės prieigos (CA) strategijas?**

Atsižvelgiant į organizacijos CA strategijas, vartotojui, kuris naudoja "Microsoft "Graph"" išteklius per jūsų taikomąją programą, gali būti užginčyti papildomos informacijos, kurios nėra iš pradžių įsigytoje prieigos atpažinimo ženklą. Tokiu atveju programa gauna 400 su *interaction_required* klaidą bandant gauti prieigos atpažinimo ženklą, arba 403 su *insufficient_claims* klaidą bandant iškviesti „Microsoft Graph“. Abiem atvejais atsakyme į klaidą yra papildomos informacijos, kurią galima pateikti įgaliotam galinį punktą, kad vartotojas galėtų užginčyti papildomą informaciją (pvz., kelių dalių autentifikavimą arba įrenginio registraciją).

- [Sąlyginių prieigos problemų sprendimas naudojant MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [„Azure Active Directory“ sąlyginės prieigos kūrėjų rekomendacijos](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
