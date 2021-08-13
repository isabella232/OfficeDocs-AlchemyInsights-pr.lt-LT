---
title: Numatytojo „Yammer“ domeno keitimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950124"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Numatytojo / pirminio „Yammer“ domeno keitimas

„Yammer“ URL nurodytas dabartinis pirminis jūsų „Yammer“ tinklo pagrindinis domeno vardas. Šis domeno vardas gali neatitikti pirminio domeno vardo, nustatyto „Office 365“ arba „Azure AD“. Veikimo būdas skiriasi, atsižvelgiant į pasirinktinių domenų, įtrauktų į nuomotoją, skaičių ir į tai, ar „Yammer“ yra palaikomos konfigūracijos (1 nuomotojas: 1 tinklas arba 1:1). Yra pasiekiama [„Yammer“ domenų ir „Office 365“](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) dokumentacija.

Dažniausia priežastis, kodėl matote neteisingą domeną, yra egzistuojantys keli „Yammer“ tinklai, kurie turi būti sujungti. [Sujungimas į vieną tinklą](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) – svarbus pirmasis veiksmas, kurį reikia atlikti naudojant tinklo perkėlimo įrankį. Atlikite tai prieš bandydami nustatyti pirminį domeną.

**Be pasirinktinių domenų**

Naujų nuomotojų atveju „Yammer“ bus naudojamas numatytasis nuomotojo domenas (pvz., fabrikam.onmicrosoft.com). Pirminis domenas nustatomas į yammer.com/fabrikam.onmicrosoft.com.

**Vienas pasirinktinis domenas**

„Yammer“ automatiškai pasirinks pasirinktinį domeną (pvz., fabrikam.com) iš nuomotojo, kaip pirminį „Yammer“ domeną. Nustatomas yammer.com/fabrikam.com. Šį keitimą atlieka domenų sinchronizavimo tarnyba ir tai gali užtrukti iki 24 valandų.

**Keli pasirinktiniai domenai**

„Yammer“ gali turėti pirminį domeną, kuris skiriasi nuo numatytojo nuomotojo domeno. Kadangi yra keli pasirinktiniai domenai, „Yammer“ nebando atspėti tinkamo domeno iš galimų. Turite užregistruoti palaikymo atvejį, kad pateiktumėte pirminio domeno vardo keitimo į jūsų pasirinktą pirminį domeną užklausą.

**Papildoma trikčių šalinimo informacija**

Kai kuriais atvejais domenai galėjo būti perkelti iš vieno nuomotojo į kitą, todėl nepavyksta sėkmingai paleisti domenų sinchronizavimo tarnybos. Galite susidurti ne tik su netinkamu pirminiu domenu, bet ir su prisijungimo ir kitomis problemomis. Norint išspręsti šią problemą, domenus gali reikėti perkelti į tinkamą tinklą, padedant „Microsoft“ palaikymo tarnybai. Šioje situacijoje reikalinga tiesioginė pagalba ir jos sprendimas gali šiek tiek užtrukti, ypač, jei yra labai ilgas domenų vardų sąrašas. Užregistruokite palaikymo atvejį, kad gautumėte pagalbos sprendžiant šių tipų problemas.

Kai dirbate su palaikymo agentu, jis patikrins, ar domenai yra patvirtinti jūsų valdomame nuomotojuje. Agentas gali užduoti papildomų su patvirtinimu susijusių klausimų apie jūsų domenus, jei jie yra įtraukti į jūsų nuomotoją, bet nepatvirtinti DNS. Kad procesas būtų spartesnis, įsitikinkite, jog domenus patvirtino DNS.
