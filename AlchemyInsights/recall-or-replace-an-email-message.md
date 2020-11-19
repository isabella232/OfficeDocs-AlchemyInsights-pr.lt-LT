---
title: Laiško atšaukimas arba pakeitimas
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353514"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Laiško atšaukimas arba pakeitimas "Microsoft 365"

- Galite **atšaukti tik tuos, kurie siunčiami į jūsų organizacijos žmones**. Pavyzdžiui, jei laiškas buvo nusiųstas į "Gmail" adresą, jo atšaukti negalėsite.
- **Iš "Outlook" kompiuteriui siunčiamų žinučių galite atšaukti tik**. Jei vartotojas siunčia laišką naudodamas "Outlook for Mac" arba internetinę "Outlook", jo atšaukti negalėsite.
- Kaip nuomotojo administratorius galite **Atšaukti vartotojų vardu esančius laiškus naudodami "PowerShell"** (daugiau informacijos rasite: [el. laiškų ieška ir naikinimas](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Negalite atšaukti laiško administravimo centre. Norėdami gauti daugiau informacijos, slinkite žemyn iki "ieškoti ir naikinti el. laiškus organizacijoje".

**Atsiųsto el. laiško atšaukimas arba pakeitimas**

1. Programos "Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.
2. Atidarykite laišką, kurį norite atšaukti. Norėdami atidaryti laišką, turite jį dukart spustelėti. Pažymėdami pranešimą, kad jis būtų rodomas skaitymo srityje, negalėsite atšaukti pranešimo.
3. Skirtuke laiškas pasirinkite **veiksmus**  >  **atšaukti šį pranešimą**.
4. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti Neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **gerai**.
5. Jei siunčiate pakaitinį pranešimą, parašykite pranešimą, tada pasirinkite **Siųsti**.
6. Laiško atšaukimo sėkmė arba gedimas priklauso nuo gavėjų parametrų programoje "Outlook".

Jei reikia daugiau informacijos, įskaitant tai, kaip patikrinti atšaukimą, žr. [pranešimo atšaukimas arba pakeitimas, kurį nusiuntėte](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Jei norite **_Ieškoti ir naikinti el. laiškus organizacijoje_**, paprasčiausia, jei esate visuotinis administratorius. Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į "e" aptikimo tvarkytuvo vaidmenų grupę arba atitikties ieškos valdymo vaidmenį. Norėdami panaikinti laišką, turite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskirtos [saugos & atitikties centre](https://protection.office.com/).

1. [Sukurkite turinio iešką](https://docs.microsoft.com/microsoft-365/compliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.
2. [Prisijunkite prie saugos & atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)".

Jei naudojate MFA (kelių dalių autentifikavimą), žiūrėkite [prisijungti prie "Microsoft 365" saugos & atitikties centro "PowerShell", naudodami kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
