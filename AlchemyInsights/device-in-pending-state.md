---
title: Įrenginio laukiama būsena
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678485"
---
# <a name="device-in-pending-state"></a>Įrenginio laukiama būsena

**Būtinosios sąlygos**

1. Jei pirmą kartą nustatote įrenginio registracijas, įsitikinkite, kad "Azure [Active Directory" ("Azure AD") peržiūrėjote Supažindinimas su įrenginių valdymu](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) "Azure AD" ("Azure AD").
2. Jei norite registruoti įrenginius į "Azure AD" tiesiogiai ir juos pateikti į "Intune", turite užtikrinti, kad [sukonfigūravote "Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) " ir pirmiausia turite [licencijavimą](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Įsitikinkite, kad turite teisę atlikti operacijas "Azure AD" ir vietiniame skelbime. Tik visuotinis administratorius "Azure AD" gali valdyti įrenginio registravimų parametrus. Be to, jei nustatote automatines registracijas vietinėje "Active Directory", turite būti "Active Directory" ir AD FS (jei taikoma) administratorius.

Hibridinis "Azure AD" prisijungimo procesas reikalauja, kad įrenginiai būtų taikomi korporatyviniame tinkle. Jis taip pat veikia per VPN, tačiau yra tam tikrų apribojimų. Mes girdėjome klientus, kuriems reikia pagalbos šalinant hibridinio "Azure AD" prisijungimo procesą pagal nuotolinio darbo aplinkybes.

**Debesies autentifikavimo aplinka (naudojant "Azure AD" slaptažodžių maišos sinchronizavimą arba Pass-per autentifikavimą)**

Šis registracijos srautas taip pat žinomas kaip "sinchronizavimo sujungimas".

Toliau aprašyta, kas nutinka registracijos proceso metu:

1. "Windows 10" aptinka tarnybos jungties taško (SCP) įrašą, kai vartotojas prisijungia prie įrenginio.

    1. Įrenginys pirmiausia bando gauti nuomotojo informaciją iš kliento "SCP" registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Daugiau informacijos ieškokite [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Jei nepavyksta, įrenginys palaiko ryšį su vietinio "Active Directory", kad gautų nuomotojo informaciją iš "SCP". Norėdami patvirtinti, kad SCP būtų galima pateikti šį [dokumentą](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Rekomenduojame įgalinti "Active Directory" SCP ir naudoti tik kliento "SCP" pradiniam patvirtinimui.

2. "Windows 10" bando palaikyti ryšį su "Azure AD" pagal sistemos kontekstą ir autentifikuoja save nuo "Azure AD".

    Galite patikrinti, ar įrenginys gali pasiekti "Microsoft" išteklius pagal sistemos paskyrą, naudodami [bandomojo įrenginio registracijos ryšio scenarijų](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. "Windows 10" generuoja vartotojo pasirašomą sertifikatą ir saugo ją po kompiuterio objektu vietiniame "Active Directory". Tam reikia, kad būtų matomas domeno valdiklis.

4. Įrenginio objektas, turintis sertifikatą, bus sinchronizuotas su "Azure AD" naudojant "Azure AD Connect". Sinchronizavimo ciklas yra kas 30 minučių pagal numatytuosius parametrus, tačiau tai priklauso nuo "Azure AD Connect" konfigūracijos. Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Šiame etape jums turėtų būti suteikta galimybė matyti temos įrenginį "**laukianti**" būsena dalyje "Azure" portalo įrenginio peilis.

6. Kitas vartotojas prisijungęs prie "Windows 10", registracija bus atlikta.

    > [!NOTE]
    > Jei esate VPN ir atsijungti/prisijungti nutraukia domeno ryšį, galite suaktyvinti registraciją neautomatiškai. Norėdami tai padaryti:
    >
    > `dsregcmd /join`Dėl administratoriaus raginimo arba nuotoliniu būdu per PSExec į kompiuterį problemą.
    >
    > Pavyzdžiui: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Jei turite įprastas "Azure Active Directory" įrenginio registravimo problemas, peržiūrėkite [įrenginių DUK](https://docs.microsoft.com/azure/active-directory/devices/faq).
