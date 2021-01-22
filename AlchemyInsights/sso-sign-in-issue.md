---
title: Sklandžios SSO prisijungimo problemos
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935175"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Sklandžios SSO prisijungimo problemos

Kai vartotojas autentifikuotas, naršyklė pereis vartotojo kredencialus, kad toje pačioje naršyklėje programa automatiškai prisijungtų prie tos pačios paskyros. Dėl to gali būti sunku kitam vartotojui arba vienam vartotojui prisiregistruoti prie kelių paskyrų viename įrenginyje. Norėdami išspręsti šią problemą: 1. Pabandykite prisijungti kitoje naršyklėje. 2. Išvalykite naršyklės talpyklą ir (arba) slapukus ir bandykite prisijungti dar kartą.

Jei vis dar kyla prisijungimo problemų, rekomenduojame nustatyti ir automatizuoti sprendimo veiksmus:

1. Įdiekite [mano programos saugiojo naršyklės plėtinį](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) , kad "Azure Active Directory" ("Azure AD") būtų lengviau diagnozuoti ir išspręsti naudojant "Azure" portalo testavimo patirtį.
2. Atkurkite klaidą naudodami "Azure" portalo taikomosios programos konfigūravimo puslapio tikrinimo patirtį. Jei norite sužinoti daugiau, skaitykite ["SAML" pagrįstų vienkartinio prisijungimo taikomųjų programų derinimas](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Jei naudojate "Azure" portalo tikrinimo patirtį su "mano Apps" saugiais naršyklės plėtiniu, galite **praleisti 4 veiksmą**.
4. Norėdami atidaryti SAML pagrįstą vienkartinio prisijungimo konfigūravimo puslapį:
    - Atidarykite " [Azure" portalą](https://portal.azure.com/) ir prisijunkite kaip **visuotinis administratorius** arba **coadmin**.
    - Atidarykite " **Azure Active Directory" plėtinį** pasirinkę **Visos tarnybos** pagrindinio kairiojo naršymo meniu viršuje.
    - Filtro ieškos lauke įveskite "Azure Active Directory" ir pasirinkite " **Azure Active Directory** " elementą.
    - Pasirinkite **įmonės taikomosios programos** iš "Azure Active Directory" kairiojoje naršymo meniu.
    - Norėdami peržiūrėti visų taikomųjų programų sąrašą, pasirinkite **visos taikomosios programos** . Jei nematote norimos programos Rodyti čia, naudokite **filtro** valdiklį **visų taikomųjų programų sąrašo** viršuje ir nustatykite parinktį **Rodyti** **visoms programoms**.
    - Pasirinkite taikomąją programą, kurią norite konfigūruoti kaip bendrąją autentifikacija.
    - Įkėlus programą, pasirinkite **bendrosios autentifikacijos** programos kairiajame naršymo meniu.
    - Pasirinkite **SAML pagrįstą SSO**.
5. Atsižvelgiant į klaidą, Sužinokite daugiau apie rekomenduojamus veiksmus, ieškokite [problemų prisijungiant prie SAML pagrįstų vienkartinio prisijungimo programų](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Norėdami pašalinti kitų vartotojų prisijungimo problemas, atsižvelkite į šiuos nurodymus:
    - [Bendras Sign-On SAML protokolas](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Kaip: prisijungimo klaidų trikčių šalinimas naudojant "Azure Active Directory" ataskaitas](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Netikėtas sutikimo raginimas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Vartotojo sutikimo klaida](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Prisijungimo iš mano programėlių problemos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Klaida programos prisijungimo puslapyje](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Prisijungimo prie "Microsoft" taikomosios programos problema](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
