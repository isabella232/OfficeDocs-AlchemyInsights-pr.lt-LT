---
title: Gaunu blokuojamą sąlyginę prieigą su domeno sujungtu įrenginiu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036702"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Gaunu blokuojamą sąlyginę prieigą su domeno sujungtu įrenginiu

**Labai Rekomenduojami įrankiai**

[Įrenginių registravimo trikčių diagnostikos priemonė](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – įrankis, padedantis pašalinti dažniausiai pasitaikančių įrenginių registravimo triktis.

[Patikrinkite įrenginio registracijos ryšio scenarijų](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – scenarijų, kuris padeda užtikrinti, kad įrenginys galėtų pasiekti įrenginio registracijos pabaigos taškus po sistemos abonementu.

" [Azure AD" įrenginio valymo scenarijus](https://github.com/mzmaili/AzureADDeviceCleanup) – scenarijus, leidžiantis ieškoti ir valdyti "pasenusių apsikeitimo" įrenginius savo aplinkoje.

Štai kelios dažniausios priežastys, kodėl sąlyginiai "Access" gali būti nepavykę įrenginio, kuris prisijungė prie domeno (hibridinio "Azure AD").

1. **Įrenginyje nėra "AZURE ad PRT"** – reikia įsitikinti, kad įrenginyje yra "Azure AD" pirminis atnaujinimo atpažinimo ženklas (PRT). Daugiau informacijos apie PRT ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Norėdami patikrinti, ar turite "Azure AD PRT", galite vykdyti `dsregcmd/status` įrenginio komandą ir patikrinti, ar "AzureAdPrt" yra lygu "Yes".

Jei "AzureAdPrt" yra "ne", patikrinkite šiuos dalykus:

- **Nesvarbu, ar turite išorinės aplinkos su AD FS ir yra nepasiekiamas iš vartotojų namų tinklo**: šiuo atveju įsitikinkite, kad jūsų "usernamemixed" pabaigos taškai pasiekiami iš ekstraneto. Jei AD FS yra už VPN, pasirūpinkite, kad vartotojai prisijungtų prie VPN ir iš naujo prisijungtų prie įrenginio. Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Ar įrenginio TPM yra klaidingas ir todėl negali autentifikuoti įrenginio**: pažymėkite "TPM. msc", kad pamatytumėte, ar TPM būsena yra "paruošta". Jei ne, paleiskite `dsregcmd/leave` ir paleiskite įrenginį iš naujo prisijungti prie "AZURE AD". Tada bandykite dar kartą. Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- Naudojate **trečiosios šalies tapatybės teikėją, nepalaikantį WS-Trust protokolo**. Kaip aprašyta mūsų dokumentuose, hibridiniai "Azure AD" įrenginiai šiuo atveju neveikia. Susisiekite su savo tapatybės teikėju.

2. **Vartotojai naudoja "Chrome" naršyklę be "Windows 10" paskyrų** arba " **Office" plėtinio "Chrome" automatiškai nenaudoja "pag" ar "Hybrid-AAD" įrenginių. "Windows"**, kuri yra su įrenginiu susietos sąlyginės prieigos strategijos, rodomas klaidos pranešimas "neregistruotasis įrenginys". Jei norite tinkamai naudoti "Chrome" naršyklę, turite įdiegti "Windows 10" paskyras arba "Office" plėtinį vartotojų "Chrome" naršyklėje per SCCM arba Intune. Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Jei negalima išplėsti plėtinio nuotoliniu būdu, praneškite vartotojams rankiniu būdu įdiegti vieną iš aukščiau nurodytų plėtinių, kad būtų galima pasiekti taikomąsias programas už įrenginių pagrindu veikiančią sąlyginę prieigą. Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Įrenginys buvo tinkamai hibridinio "AZURE AD", bet jis buvo netyčia panaikintas arba išjungtas dėl sinchronizavimo pasikeitimų "AZURE AD Connect" arba "Azure" portale**: jei taip nutinka, įrenginio objektas nebėra atpažįstamas kaip visiškai sujungtas įrenginys, nors "Azureadsujungtos" ir "PRT" būsena rodoma kaip tinkama įrenginyje.

Norėdami išspręsti šią problemą, paleiskite `dsregcmd/leave` paveiktus įrenginius ir leisti jiems vėl prisijungti prie "AZURE AD". Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Jei jūsų įrenginiai yra "Windows 10", "1809" naujinime, naudodami VPN/debesies tarpinį serverį ir matysite problemas "AzureAdPrt" arba bet kurią taikomąją programą su SSO problema ("Outlook" nesusijungia su pašto dėžute, net jei turėjote "PRT"), įsitikinkite, kad turite šį pataisos [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) arba balandžio kaupiamojo naujinimo [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , kad išvengtumėte šių mašinų PRT gedimų

















