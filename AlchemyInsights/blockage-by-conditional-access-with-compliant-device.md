---
title: Gaunu blokuojamą sąlyginę prieigą su suderinamu įrenginiu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035998"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Gaunu blokuojamą sąlyginę prieigą su suderinamu įrenginiu

**Labai Rekomenduojami įrankiai**

- [Įrenginių registravimo trikčių diagnostikos priemonė](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – išsamus įrankis, padedantis pašalinti Dažniausias įrenginio registravimo problemas.
- [Patikrinkite įrenginio registracijos ryšio scenarijų](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – įrankį, naudojamą užtikrinti, kad įrenginys galėtų pasiekti įrenginio registracijos pabaigos taškus po sistemos abonementu.
- " [Azure AD" įrenginio valymo scenarijus](https://github.com/mzmaili/AzureADDeviceCleanup) – įrankis, naudojamas ieškant ir tvarkant "pasenusių apsikeitimo" įrenginius jūsų aplinkoje.

Čia pateikiamos kelios dažniausios priežastys, kodėl sąlyginės prieigos galimybė gali nepavykti dėl suderinamo įrenginio, arba kodėl jūsų vartotojai gali **gauti iš čia** gauto pranešimo prisijungimo užklausoje prie organizacijos išteklių.

1. **Įrenginio nėra būtinoje įrenginio būsenoje su MDM**:

Patikrinkite, ar įrenginys užregistruotas su patvirtintu MDM tiekėju, pvz., Intune ir *pažymėtas kaip suderinamas*. Daugiau informacijos apie Intune Peržiūrėkite šį [dokumentą](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Norėdami geriau suprasti įrenginio atitiktį ir Intune, žiūrėkite [naudoti atitikties strategiją, kad nustatytumėte įrenginių, kuriuos tvarkote naudodami Intune, taisykles](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Jei kyla problemų naudojant įrenginį su Intune, raskite trikčių šalinimo išsamią informaciją trikčių šalinimo [įrenginyje "Microsoft"](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Norėdami gauti daugiau "Intune" palaikymo, sukurkite palaikymo užklausą. Norėdami tai padaryti, apsilankykite " [Intune" žinyno ir palaikymo puslapyje](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Įrenginys neprijungtas prie organizacijos tinklo**:

Norint pasiekti organizacijos išteklius, įrenginys turi būti prijungtas prie organizacijos tinklo, naudojant tiesioginį ryšį arba virtualaus privačiojo tinklo (VPN), taip pat prisijungė prie vietinio arba "Azure Active Directory". Norėdami prisijungti prie darbo įrenginio organizacijos tinkle, žiūrėkite prisijungti prie [savo darbo įrenginio prie savo organizacijos tinklo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Norėdami užregistruoti asmeninį/"BYOD" įrenginį, žiūrėkite [savo organizacijos tinkle užregistruokite savo asmeninį įrenginį](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Norėdami patikrinti, ar įrenginys prisijungė prie tinklo, galite atlikti čia pateiktus veiksmus, skirtus registruotiems įrenginiams [čia](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) arba darbo įrenginiams [čia](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Jei norite, kad būtų taikoma organizacijos tinklo ryšio problema, vadovaukitės toliau pateikiamais nurodymais:

    1. Prisijunkite prie "Windows" naudodami savo darbo arba mokymo įstaigos paskyrą, pvz., alain@contoso.com.
    2. Prisijunkite prie savo organizacijos tinklo per VPN arba "DirectAccess".
    3. Kai prisijungsite, paspauskite **"Windows" logotipo klavišą + L** , kad užrakintumėte įrenginį.
    4. Atrakinkite įrenginį naudodami darbo arba mokymo įstaigos paskyrą, tada bandykite pasiekti probleminę programą arba paslaugą dar kartą.

Jei matote, kad dar kartą **čia negalite gauti iš čia** pateikto klaidos pranešimo, problema yra tikimybė kitur.

3. **Operacinė sistema** nepalaikoma:

Įsitikinkite, kad naudojate palaikomą operacinės sistemos versiją, įskaitant:

- **"Windows" klientas**: "Windows 7" arba vėlesnė versija

- **"Windows Server**": "Windows server" 2008 R2 arba vėlesnė versija

- **MacOS**: MacOS X arba vėlesnė versija

- **"Android" ir "iOS**": naujausia "Android" ir "iOS" mobiliųjų operacinių sistemų versija

4. **Žiniatinklio naršyklė nepalaikoma**:

Ieškokite palaikomų naršyklių toliau. Norint naudoti "Chrome" palaikymą su "Windows" 1703 arba naujesnėmis versijomis, būtinas "Windows 10" paskyrų plėtinys. Kad būtų galima tinkamai perduoti įrenginio atitikties informaciją, vartotojui reikia prijungti prie "Edge" 85 +. Daugiau informacijos rasite [čia](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **"Windows 10**": "Microsoft Edge", "Internet Explorer", "Chrome"
- **"Windows 8"/"8,1"**: "Internet Explorer", chromas
- **"Windows 7"**: "Internet Explorer", "Chrome"
- " **ios**": "Microsoft Edge", Intune valdoma naršyklė, "Safari"
- "Android **": "Microsoft Edge"**: Intune valdoma naršyklė, "Chrome"
- **"Windows Phone**": "Microsoft Edge", "Internet Explorer"
- **"Windows Server 2019**": "Microsoft Edge", "Internet Explorer", "Chrome"
- **"Windows Server 2016": "** Internet Explorer"
- **"Windows Server 2012 R2": "** Internet Explorer"
- **"Windows Server 2008 R2": "** Internet Explorer"
- " **macOS**": "Chrome", "Safari"

Rasti daugiau informacijos apie tai, kaip [čia](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation) **negalite gauti** pranešimo ir trikčių diagnostikos veiksmų.
