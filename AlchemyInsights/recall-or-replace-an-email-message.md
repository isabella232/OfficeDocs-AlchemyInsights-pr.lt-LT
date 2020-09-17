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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799212"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Laiško atšaukimas arba pakeitimas "Microsoft 365"

- Galite **atšaukti tik tuos, kurie siunčiami į jūsų organizacijos žmones**. Jei laiškas buvo išsiųstas į "Gmail" adresą, pvz., jo atšaukti negalėsite.
- Galite **atšaukti tik iš "Outlook 2016" kompiuteriui atsiųstus tekstinius** Jei vartotojas siunčia laišką naudodamas "Outlook for Mac" arba internetinę "Outlook", jo atšaukti negalėsite.
- Jei esate administratorius, galite **Atšaukti vartotojų vardu siunčiamus, naudodami "PowerShell"**. Negalite atšaukti laiško administravimo centre. Norėdami gauti daugiau informacijos, slinkite žemyn iki "ieškoti ir naikinti el. laiškus organizacijoje".

**Atsiųsto el. laiško atšaukimas arba pakeitimas**

1. Programos "Outlook" lango kairėje esančioje aplankų srityje pasirinkite aplanką Išsiųsta.
2. Atidarykite laišką, kurį norite atšaukti. Norėdami atidaryti laišką, turite jį dukart spustelėti. Pažymėdami pranešimą, kad jis būtų rodomas skaitymo srityje, negalėsite atšaukti pranešimo.
3. Skirtuke laiškas pasirinkite **veiksmus**  >  **atšaukti šį pranešimą**.
4. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti Neskaitytas kopijas ir pakeisti nauju pranešimu**, tada pasirinkite **gerai**.
5. Jei siunčiate pakaitinį pranešimą, parašykite pranešimą, tada pasirinkite **Siųsti**.
6. Laiško atšaukimo sėkmė arba gedimas priklauso nuo gavėjų parametrų programoje "Outlook".

Jei reikia daugiau informacijos, įskaitant tai, kaip patikrinti atšaukimą, žr. [pranešimo atšaukimas arba pakeitimas, kurį nusiuntėte](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Savo organizacijos el. laiškų ieška ir naikinimas*** Jei norite ieškoti ir naikinti el. laiškus organizacijoje, paprasčiausia, jei esate visuotinis administratorius. Jei nesate visuotinis administratorius, jūsų abonementas turi būti įtrauktas į "e" aptikimo tvarkytuvo vaidmenų grupę arba atitikties ieškos valdymo vaidmenį. Norėdami panaikinti laišką, turite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskirtos [saugos & atitikties centre](https://protection.office.com/).

1. [Sukurkite turinio iešką](https://docs.microsoft.com/microsoft-365/compliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.
2. [Prisijunkite prie saugos & atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)". 

Jei naudojate MFA, ieškokite [prisijungimas prie "Microsoft 365" saugos & atitikties centro "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
