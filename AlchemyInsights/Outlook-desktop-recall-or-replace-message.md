---
title: Outlook Darbalaukio atšaukimas arba el. laiško keitimas
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918403"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>El. laiško atšaukimas Outlook keitimas

- Kaip administratorius, galite atšaukti **pranešimus vartotojų vardu naudodami "PowerShell".** Negalite atšaukti pranešimų iš administravimo centro.
- Galite atšaukti **tik laiškus, siunčiamus jūsų organizacijos žmonėms.** Pavyzdžiui, jei pranešimas buvo išsiųstas "Gmail" adresu, jo atšaukti negalite.
- Galite atšaukti **tik laiškus, išsiųstus iš Outlook 2016 kompiuteryje.** Jei vartotojas siunčia pranešimą naudodamas "Outlook Mac" arba "internetinė "Outlook"", jo atšaukti negalite.

Norėdami atšaukti arba pakeisti el. laišką:

1. Aplanko srityje, esančioje kairėje lango Outlook pasirinkite aplanką Išsiųsta.
1. Dukart spustelėkite pranešimą, kurį norite atšaukti, kad jį atidarytumėte.
1. Pasirinkite skirtuką **Pranešimas,** tada pasirinkite **Veiksmai** Atšaukti  >  **šį pranešimą**.
1. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti neskaitytas** kopijas ir pakeisti nauju pranešimu , tada pasirinkite **Gerai**.
1. Jei siunčiate pakaitinį pranešimą, sukurkite pranešimą, tada pasirinkite **Siųsti**.
1. Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjo parametrų Outlook. Norėdami sužinoti, kaip patikrinti atšaukimą, žr. [šį straipsnį](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

El. laiškų ieška ir naikinimas organizacijoje

- Jei esate ne visuotinis administratorius, jūsų paskyra turi būti įtraukta į el. duomenų aptikimo tvarkytuvo vaidmenį arba atitikties ieškos valdymo vaidmenį ieškant pranešimų. Norėdami panaikinti laiškus, turėsite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskiriamos saugos [ir atitikties centre.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Sukurkite turinio iešką,](https://docs.microsoft.com/microsoft-365/compliance/content-search) kad rastumėte pranešimą, kurį norite panaikinti.
- [Prisijungimas į saugos ir atitikties centro "PowerShell".](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Jei naudojate kelių dalių autentifikavimą, žr. Prisijungimas Microsoft 365 ir atitikties centro ["PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).