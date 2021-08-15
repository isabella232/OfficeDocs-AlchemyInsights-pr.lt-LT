---
title: El. laiško atšaukimas arba keitimas
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024394"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>El. laiško atšaukimas arba keitimas Microsoft 365

- Galite atšaukti **tik laiškus, siunčiamus jūsų organizacijos žmonėms.** Pavyzdžiui, jei pranešimas buvo išsiųstas "Gmail" adresu, jo atšaukti negalite.
- Galite atšaukti **tik iš kompiuterio Outlook laiškus.** Jei vartotojas siunčia pranešimą naudodamas "Outlook Mac" arba "internetinė "Outlook"", jo atšaukti negalite.
- Kaip nuomotojo administratorius, galite atšaukti pranešimus vartotojų vardu naudodami **"PowerShell"** (Daugiau informacijos žr.: [El. laiškų ieška ir naikinimas).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Negalite atšaukti pranešimų iš administravimo centro. Norėdami gauti daugiau informacijos, slinkite žemyn iki "Ieškoti ir naikinti el. laiškus savo organizacijoje".

**Išsiųsto el. laiško atšaukimas arba keitimas**

1. Aplankų srityje, kairėje lango Outlook pasirinkite aplanką Išsiųsta.
2. Atidarykite pranešimą, kurį norite atšaukti. Norėdami atidaryti pranešimą, turite dukart spustelėti. Pažymėjus pranešimą, kad jis būtų rodomas skaitymo srityje, pranešimo atšaukti negalėsite.
3. Skirtuke Pranešimas pasirinkite **Veiksmai** Atšaukti  >  **šį pranešimą**.
4. Pasirinkite **Naikinti neskaitytas šio pranešimo kopijas** arba **Naikinti neskaitytas** kopijas ir pakeisti nauju pranešimu , tada pasirinkite **Gerai**.
5. Jei siunčiate pakaitinį pranešimą, sukurkite pranešimą, tada pasirinkite **Siųsti**.
6. Pranešimo atšaukimo sėkmė arba nesėkmė priklauso nuo gavėjų parametrų Outlook.

Daugiau informacijos, įskaitant tai, kaip patikrinti atšaukimą, [žr. Išsiųsto el. laiško atšaukimas arba keitimas](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Norint ieškoti ir naikinti el. laiškus*** organizacijoje, paprasčiausia, jei esate visuotinis administratorius. Jei esate ne visuotinis administratorius, jūsų paskyra turi būti įtraukta į el. duomenų aptikimo tvarkytuvo vaidmenų grupę arba į atitikties ieškos valdymo vaidmenį. Norėdami panaikinti laiškus, turėsite prisijungti prie organizacijos valdymo vaidmenų grupės arba ieškos ir valymo valdymo vaidmens. Šių vaidmenų teisės priskiriamos saugos ir [& centre.](https://protection.office.com/)

1. [Sukurkite turinio iešką,](https://docs.microsoft.com/microsoft-365/compliance/content-search) kad rastumėte pranešimą, kurį norite panaikinti.
2. [Prisijungimas į saugos & "PowerShell".](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Jei naudojate MFA (kelių dalių autentifikavimą), žr. ["Prisijungimas to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
