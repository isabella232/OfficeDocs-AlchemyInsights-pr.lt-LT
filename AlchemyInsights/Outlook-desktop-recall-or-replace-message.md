---
title: "\"Outlook\" darbalaukio atšaukimas arba el. laiško keitimas"
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687518"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>"Outlook" el. laiško atšaukimas arba keitimas

- Kaip administratorius, galite **atšaukti pranešimus vartotojų vardu naudodami "PowerShell".** Negalite atšaukti pranešimų iš administravimo centro.
- Galite **atšaukti tik tuos pranešimus, kurie siunčiami jūsų organizacijos žmonėms**. Pavyzdžiui, jei pranešimas buvo išsiųstas "Gmail" adresu, jo atšaukti negalėsite.
- Galite **atšaukti tik pranešimus, išsiųstus iš "Outlook 2016" kompiuteryje**. Jei vartotojas siunčia pranešimą naudodamas "Outlook for Mac" arba "Outlook" žiniatinklyje, jo atšaukti negalite.

Norėdami atšaukti arba pakeisti el. laišką:

1. "Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.
1. Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.
1. Pasirinkite skirtuką **Pranešimas,** tada pasirinkite **Veiksmai** > **Atšaukti šį pranešimą**.
1. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **Gerai**.
1. Jei siunčiate pakaitinį pranešimą, sukurkite pranešimą, tada pasirinkite **Siųsti**.
1. Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjo parametrų programoje "Outlook". Veiksmus, kuriuos reikia patikrinti atšaukimo, ieškokite [šiame straipsnyje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

El. laiškų ieška ir naikinimas organizacijoje

- Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į el. duomenų aptikimo tvarkytuvo vaidmenį arba atitikties ieškos valdymo vaidmenį, kad būtų ieškoma pranešimų. Norėdami panaikinti pranešimus, turėsite prisijungti prie vaidmenų grupės Organizacijos valdymas arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskiriamos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Sukurkite turinio iešką,](https://docs.microsoft.com/office365/securitycompliance/content-search) kad rastumėte naikintiną pranešimą.
- [Prisijunkite prie saugos ir atitikties centro "PowerShell".](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Jei naudojate kelių dalių autentifikavimą, [žr.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)