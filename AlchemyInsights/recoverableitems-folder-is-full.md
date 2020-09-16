---
title: "\"1336\" Recoverableitonų aplankas yra pilnas"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741275"
---
# <a name="the-recoverable-items-folder-is-full"></a>Aplankas Atkuriami elementai yra pilnas

"Exchange Online" pašto dėžutėms numatytoji aplanko atkuriamų elementų saugyklos riba yra 30 GB. Aplanko Atkuriami elementai saugyklos limitas automatiškai padidinamas iki 100 GB, jei pašto dėžutė įtraukta į sulaikymą dėl bylinėjimosi, "el. Discovery" sulaikyta arba priskiriama saugojimo strategijai.

Kai atkuriamų elementų aplankas pasiekia saugyklos limitą, pašto dėžutės funkcijos veikia šiais būdais:

- Vartotojas negali panaikinti pašto dėžutės elementų.

- Valdomojo aplanko pagalbinė priemonė negali panaikinti elementų, pagrįstų saugojimo žyme arba valdomais aplanko parametrais.

- Pašto dėžučių, kurioms įgalintas vieno elemento atkūrimas arba kurios sulaikytos, kopijavimo ir rašymo puslapio apsaugos procesas negali išlaikyti vartotojo redaguotų elementų versijų.

- Pašto dėžučių, kurioms įgalintas pašto dėžučių audito registravimas, pašto dėžučių audito žurnalo įrašus galima įrašyti aplanke Atkuriami elementai.

Jei pašto dėžutės nėra sulaikytos, administratoriai gali naudoti komandą " `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell", kad panaikintų elementų aplanke Atkuriami elementai. Norėdami gauti daugiau informacijos žr. toliau nurodytas temas:

- [Žinučių ieška ir naikinimas](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Ieška – pašto dėžutė](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Jei pašto dėžutės yra sulaikytos, administratoriai turi pašalinti sulaikymą prieš panaikindami elementus iš aplanko Atkuriami elementai. Daugiau informacijos ieškokite [elementų naikinimas nuotolinėmis duomenų saugyklomis pagrįstų pašto dėžučių aplanke Atkuriami elementai](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Norėdami padėti apsisaugoti nuo aplanko Atkuriami elementai iš dalies, administratoriai gali padidinti aplanko atkuriamų elementų saugyklos limitą ir nustatyti pašto dėžučių saugojimo strategiją, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo pašto dėžutę. Peržiūrėkite ["sulaikyti" pašto dėžučių grąžinamos dalies kvotas](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
