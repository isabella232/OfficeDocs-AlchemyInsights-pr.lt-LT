---
title: Gaunu užblokuotą sąlyginės prieigos su suderinamu įrenginiu
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019156"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Gaunu užblokuotą sąlyginės prieigos su suderinamu įrenginiu

**Labai rekomenduojami įrankiai**

- [Įrenginių registracijos trikčių diagnostikos įrankis](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – išsamus įrankis, padedantis šalinti dažniausiai pasitaikančią įrenginio registracijos problemą.
- [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.
- ["Azure AD" įrenginio valymo scenarijus](https://github.com/mzmaili/AzureADDeviceCleanup) – įrankis, naudojamas ieškoti ir valdyti pasenusius įrenginius jūsų aplinkoje.

Toliau pateikiame keletą dažnai pasitaikančių priežasčių, kodėl sąlyginė prieiga gali  nepavykti dėl suderinamo įrenginio arba kodėl gali būti, kad vartotojai gali gauti iš čia pranešimo, kai prisijungiate prie organizacijos išteklių.

1. **Įrenginio būsena nebūtina su MDM:**

Patikrinkite, ar įrenginys yra įtrauktas į patvirtintą MDM teikėją, pvz., "Intune" *ir pažymėtas kaip suderinamas*. Daugiau informacijos apie "Intune" žr. šiame [dokumente](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Norėdami geriau suprasti įrenginių atitiktį ir "Intune", naudokite atitikties strategiją, kad nustatytų taisykles [įrenginiams, kuriuos valdote naudodami "Intune".](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Jei kyla problemų užregistruojant įrenginį naudojant "Intune", raskite trikčių diagnostikos informaciją skyriuje Įrenginio registracijos [trikčių diagnostika "Microsoft".](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Norėdami gauti daugiau "Intune" palaikymo, sukurkite palaikymo užklausą. Norėdami tai padaryti, apsilankykite ["Intune" žinyno ir palaikymo puslapyje](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Įrenginys neprijungtas prie organizacijų tinklo:**

Norint pasiekti organizacijos išteklius, įrenginys turi būti prijungtas prie organizacijos tinklo tiesioginiu ryšiu arba virtualiuoju privačiuoju tinklu (VPN) ir taip pat prijungtas prie vietinio arba "Azure Active Directory". Norėdami prisijungti prie darbo įrenginio prie organizacijos tinklo, žr. Darbo [įrenginio prisijungimas prie organizacijos tinklo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Norėdami užregistruoti asmeninį / BYOD įrenginį, žr. Asmeninio [įrenginio registravimas organizacijos tinkle](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Norėdami patikrinti, ar įrenginys prisijungė prie tinklo, čia [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) arba darbo įrenginiuose galite atlikti registruotų įrenginių [veiksmus.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Norėdami išspręsti organizacijos tinklo ryšio problemą, vadovaukitės toliau pateikiamomis gairėmis:

    1. Prisijunkite prie Windows naudodami darbo arba mokymo įstaigos paskyrą, pvz., alain@contoso.com.
    2. Prisijungimas į organizacijos tinklą naudodami VPN arba "DirectAccess".
    3. Kai prisijungsite, paspauskite **"Windows" logotipo klavišą + L, kad** užrakintų įrenginį.
    4. Atrakinkite įrenginį naudodami darbo arba mokymo įstaigos paskyrą, tada bandykite dar kartą pasiekti probleminę programą ar tarnybą.

Jei matote klaidos **pranešimą Čia negalite ten** patekti dar kartą, problema gali kilti kitur.

3. **Operacinė sistema nepalaikoma:**

Įsitikinkite, kad naudojate palaikomą operacinės sistemos versiją, įskaitant:

- **Windows Klientas:** Windows 7 arba naujesnė versija

- **Windows Server:** Windows Server 2008 R2" arba naujesnė versija

- **"macOS":**"macOS X" arba naujesnė versija

- **"Android" ir "iOS":** naujausia "Android" ir "iOS" mobiliųjų operacinių sistemų versija

4. **Žiniatinklio naršyklė nepalaikoma:**

Toliau rasite palaikomas naršykles. Jei reikia "Chrome" palaikymo Windows 1703 arba naujesnėse versijose, būtina Windows 10 paskyrų plėtinį. Naudojant "Edge 85+", vartotojas turi būti prisijungęs, kad tinkamai perdytų įrenginio atitikties informaciją. Daugiau informacijos žr. [čia](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10:** Microsoft Edge, "Internet Explorer", "Chrome"
- **"Windows 8" / 8.1**: "Internet Explorer", "Chrome"
- **Windows 7: "Internet** Explorer", "Chrome"
- **"iOS":**"Microsoft Edge", "Intune" valdoma naršyklė, "Safari"
- **"Android":** **Microsoft Edge**: "Intune" valdoma naršyklė, "Chrome"
- **"Windows Phone":** Microsoft Edge, "Internet Explorer"
- **Windows Server 2019:** Microsoft Edge, "Internet Explorer", "Chrome"
- **Windows Server 2016"**: "Internet Explorer"
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **"macOS":**"Chrome", "Safari"

Raskite daugiau informacijos apie **tai, kad čia negalite gauti pranešimo** ir trikčių šalinimo [veiksmų.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
