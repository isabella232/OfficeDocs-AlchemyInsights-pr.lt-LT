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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984585"
---
# <a name="application-errors"></a>Taikomosios programos klaidos

Ieškote informacijos apie " **Aadsts" klaidų kodus** , kuriuos grąžino "Azure Active Directory" ("Azure AD") saugos atpažinimo ženklų tarnyba (STS)? Perskaitykite " [AZURE AD" autentifikavimo ir autorizavimo klaidų kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , kad rastumėte AADSTS klaidų aprašus, pataisymus ir kai kuriuos siūlomus sprendimo būdus.

Autorizavimo klaidos gali kilti dėl kelių skirtingų problemų, kurių dauguma generuoja "401" arba "403" klaidą. Pavyzdžiui, toliau nurodyti būdai gali sukelti autorizavimo klaidas:

- Neteisingi [prieigos žetono įsigijimo srautai](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Netinkamai sukonfigūruotos [teisių aprėptis](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) stoka

Norėdami išspręsti įprastas autorizavimo klaidas, išbandykite toliau pateiktus veiksmus, kurie geriausiai atitinka gavimo klaidą. Gali būti taikoma daugiau nei viena.

**401 Neleistina klaida: ar jūsų žetonas galioja?**

Įsitikinkite, kad jūsų taikomoji programa pateikia tinkamą prieigos žetoną į "Microsoft Graph" kaip užklausos dalį. Ši klaida dažnai reiškia, kad "Access" atpažinimo ženklas gali trūkti HTTP autentifikavimo užklausos antraštėje arba kad atpažinimo ženklas negalioja arba nebegalioja. Primygtinai rekomenduojame naudoti ["Microsoft" autentifikavimo biblioteką (MSAL) "Access"](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) atpažinimo ženklų įsigijimui. Be to, ši klaida gali įvykti, jei bandote naudoti įgaliotojo prieigos žetoną, suteiktą asmeniniam "Microsoft" abonementui, kad pasiektumėte API, kuris palaiko tik darbo arba mokymo įstaigos paskyras (organizacijos paskyras).

**403 Forbidden klaida: pasirinkote tinkamą teisių rinkinį?**

Patikrinkite, ar prašėte tinkamą teisių rinkinį pagal "Microsoft Graph" API taikomųjų programų iškvietimus. Rekomenduojamos mažiausiai privilegijuotos teisės pateikiamos visose "Microsoft Graph" API nuorodų metodo temose. Be to, šios teisės turi būti suteiktos taikomajai programai pagal vartotoją arba administratorių. Teisių suteikimas paprastai įvyksta dėl sutikimo puslapio arba teisių suteikimo naudojant "Azure" portalo taikomosios programos registravimo diską. Taikomosios programos **parametrų** ašmenys spustelėkite **reikiamas teises**, tada spustelėkite **suteikti teises**.

- ["Microsoft Graph" teisės](https://docs.microsoft.com/graph/permissions-reference) 
- ["Azure AD" teisių ir sutikimo supratimas](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Forbidden klaida: ar jūsų programa įsigyja atpažinimo ženklą, kad atitiktų pasirinktas teises?**

Įsitikinkite, kad prašoma arba suteikta teisių rūšis atitinka jūsų taikomosios programos "Access" atpažinimo ženklo tipą. Galite prašyti ir suteikti taikomosios programos teises, bet naudoti interaktyvius interaktyviojo kodo srauto atpažinimo ženklus, o ne kliento kredencialų srauto atpažinimo ženklus, arba prašyti ir suteikti įgaliotasis teises, bet naudoti kliento kredencialų srauto atpažinimo ženklus vietoj įgaliotojo kodo srautų žetonų.

- [Gaukite prieigą vartotojų ir įgaliotų teisių vardu](https://docs.microsoft.com/graph/auth_v2_user) 
- ["Azure AD v 2.0" – "OAuth" 2,0 autorizavimo kodo srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Gaukite "Access" nenaudodami vartotojo (Daemon Service) ir taikomosios programos teisių](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0 kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 uždrausta klaida: slaptažodžio nustatymas iš naujo**

Šiuo metu nėra taikomųjų programų teisių demono paslaugų, kurios leidžia iš naujo nustatyti vartotojų slaptažodžius. Šios API palaikomos tik naudojant interaktyvius įgaliotojo kodo srautus su prisijungusiems administratoriui.

- ["Microsoft Graph" teisės](https://docs.microsoft.com/graph/permissions-reference)

**403 uždrausta: ar vartotojas turi prieigą ir jie yra licencijuoti?**

Jei tai yra įgaliotasis kodo srautai, "Microsoft Graph" įvertina, ar užklausa yra leistina pagal programai suteiktas teises ir teises, kurias prisijungęs vartotojas turi. Paprastai ši klaida nurodo, kad vartotojas nėra pakankamai privilegijuotas, kad galėtų atlikti užklausą, arba vartotojas nėra licencijuotas duomenims, kurie yra pasiekiami. Užklausą gali sėkmingai atlikti tik vartotojai, turintys reikiamas teises arba licencijas.

**403 uždrausta: ar pasirinkote tinkamą išteklių API?**

API paslaugos, pvz., "Microsoft Graph", tikrina, kad "Access" žetono reikalavimas (auditorija) sutampa su reikšme, kurią ji tikisi sau, o jei ne, tai lemia 403 Forbidden klaida. Dažna klaida dėl šios klaidos bando naudoti atpažinimo ženklą, įsigytą "Azure AD Graph" API, "Outlook" API arba "SharePoint"/"OneDrive" API, kad paskambintumėte į "Microsoft Graph" (arba atvirkščiai). Įsitikinkite, kad išteklių (arba aprėpties) jūsų programa įgyja atpažinimo ženklą, atitinkantį API, kurį skambina programa.

**400 netinkama užklausa arba 403 uždrausta: ar vartotojas laikosi savo organizacijos sąlyginės prieigos (CA) strategijų?**

Atsižvelgiant į organizacijos CA politiką, vartotojui prieigą prie "Microsoft Graph" išteklių galima ginčyti naudojant papildomą informaciją, kuri nėra jūsų taikomosios programos "Access" atpažinimo ženkle. Šiuo atveju programa gauna 400 su *interaction_required* klaida "Access" atpažinimo ženklų įsigijimo metu arba 403 su *insufficient_claims* klaida, kai skambinama į "Microsoft Graph". Abiem atvejais klaidos atsakyme yra papildomos informacijos, kuri gali būti pateikta galinį punktą, kad vartotojas galėtų pateikti papildomos informacijos (pvz., kelių dalių autentifikavimą arba įrenginio registraciją).

- [Sąlyginės prieigos iššūkių naudojimas naudojant MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- ["Azure Active Directory" sąlyginės prieigos kūrėjo gairės](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
