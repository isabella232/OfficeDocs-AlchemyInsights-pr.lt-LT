---
title: "\"Outlook Desktop\" atšaukimas arba pakeitimas el. laiško"
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496119"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>"Outlook" el. laiško atšaukimas arba keitimas

- Kaip administratorius, galite **priminti pranešimus vartotojų vardu naudojant PowerShell**. Negalite atšaukti pranešimų iš administravimo centro.
- Galite **atšaukti tik tuos pranešimus, kurie siunčiami jūsų organizacijos žmonėms**. Jei pranešimas buvo išsiųstas "Gmail" adresu, pavyzdžiui, jo atšaukti negalėsite.
- Galite **tik atšaukti pranešimus, išsiųstus iš "Outlook 2016" kompiuteryje**. Jei naudotojas siunčia pranešimą naudodamas "Outlook for Mac" arba "Outlook" žiniatinklyje, jo atšaukti negalite.

Jei norite atšaukti arba pakeisti el. laišką:

1. Kairėje "Outlook" lango aplanko srityje pasirinkite aplanką Išsiųsta.
1. Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.
1. Pasirinkite skirtuką **pranešimas** , tada pasirinkite **veiksmai** > **prisiminti šį pranešimą**.
1. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **panaikinkite Neskaitytas kopijas ir pakeiskite nauju pranešimu**, tada pasirinkite **gerai**.
1. Jei siunčiate pakaitinį pranešimą, parašykite pranešimą, tada pasirinkite **Siųsti**.
1. Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjo nustatymų "Outlook". Norėdami sužinoti apie atšaukimo veiksmus, skaitykite [šį straipsnį](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Ieškoti ir naikinti el. laiškus organizacijoje

- Jei nesate visuotinis administratorius, jūsų abonementas turi būti pridėtas prie eDiscovery Manager vaidmens arba atitikties ieškos valdymo vaidmens ieškant pranešimų. Norėdami panaikinti pranešimus, turėsite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskiriamos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Sukurkite turinio iešką](https://docs.microsoft.com/office365/securitycompliance/content-search) , kad rastumėte naikindami pranešimą.
- [Prisijungti prie saugos ir atitikties centro "PowerShell"](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Jei naudojate kelių dalių autentifikavimą, peržiūrėkite [prisijungti prie "Office 365" saugos ir atitikties centro "PowerShell" naudodami kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).