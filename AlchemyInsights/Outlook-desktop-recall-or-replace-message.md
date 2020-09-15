---
title: "\"Outlook\" kompiuterio atšaukimas arba pranešimo apie laišką keitimas"
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663998"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>"Outlook" el. laiško atšaukimas arba pakeitimas

- Kaip administratorius galite **Atšaukti vartotojų vardu naudodami "PowerShell"**. Negalite atšaukti laiško administravimo centre.
- Galite **atšaukti tik tuos, kurie siunčiami į jūsų organizacijos žmones**. Jei laiškas buvo išsiųstas į "Gmail" adresą, pvz., jo atšaukti negalėsite.
- Galite **tik atšaukti iš "Outlook 2016" išsiųstus "PC"**. Jei vartotojas siunčia laišką naudodamas "Outlook for Mac" arba internetinę "Outlook", jo atšaukti negalėsite.

Norėdami atšaukti arba pakeisti el. laišką:

1. Programos "Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.
1. Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.
1. Pasirinkite skirtuką **pranešimas** , tada pasirinkite **veiksmai**  >  **atšaukti šį pranešimą**.
1. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti Neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **gerai**.
1. Jei siunčiate pakaitinį pranešimą, parašykite laišką ir pasirinkite **Siųsti**.
1. Laiško atšaukimo sėkmė arba gedimas priklauso nuo gavėjo parametrų programoje "Outlook". Norėdami patikrinti, ar yra atšaukimo veiksmų, peržiūrėkite [šį straipsnį](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Savo organizacijos el. laiškų ieška ir naikinimas

- Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į "e. Discovery Manager" vaidmenį arba atitikties ieškos valdymą, kad būtų ieškoma žinučių. Norėdami panaikinti laišką, turite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskirtos [saugos ir atitikties centre](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Sukurkite turinio iešką](https://docs.microsoft.com/microsoft-365/compliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.
- [Prisijunkite prie saugos ir atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)".

Jei naudojate kelių dalių autentifikavimą, ieškokite [prisijungimas prie "Microsoft" 365 saugos ir atitikties centro "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).