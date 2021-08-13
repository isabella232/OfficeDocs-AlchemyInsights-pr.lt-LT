---
title: 1336 Atkuriamų elementų aplankas yra pilnas
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061764"
---
# <a name="the-recoverable-items-folder-is-full"></a>Aplankas Atkuriami elementai yra pilnas

Pašto Exchange Online numatytasis aplanko Atkuriami elementai saugyklos limitas yra 30 GB. Aplanko Atkuriami elementai saugyklos limitas automatiškai padidinamas iki 100 GB, jei pašto dėžutė yra sulaikyta dėl bylinėjimosi, el. duomenų aptikimo arba priskiriama saugojimo strategijai.

Kai atkuriamų elementų aplankas pasiekia saugyklos limitą, pašto dėžutės funkcijoms įtakos turi šie būdai:

- Vartotojas negali panaikinti elementų iš pašto dėžutės.

- Valdomų aplankų pagalbinė priemonė negali panaikinti elementų pagal saugojimo žymę arba valdomo aplanko parametrus.

- Pašto dėžutėse, kuriose įjungtas arba sulaikytas vieno elemento atkūrimas, kopijavimo ir rašymo puslapio apsaugos procesas negali išlaikyti vartotojo redaguotų elementų versijų.

- Pašto dėžučių, kurių pašto dėžučių audito registravimas įgalintas, pašto dėžučių audito žurnalo įrašų negalima įrašyti aplanko Atkuriami elementai poaplankyje Auditai.

Jei pašto dėžutės nėra sulaikytos, administratoriai gali naudoti "PowerShell" Exchange Online komandą, kad panaikintų elementus `Search-Mailbox -SearchDumpsterOnly -DeleteContent` aplanke Atkuriami elementai. Norėdami gauti daugiau informacijos žr. toliau nurodytas temas:

- [Laiškų ieška ir naikinimas](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Sulaikytų pašto dėžučių atveju administratoriai turi pašalinti sulaikytus elementus, kad galėtų panaikinti elementus iš aplanko Atkuriami elementai. Daugiau informacijos žr. [Sulaikytų debesies pašto dėžučių aplanke Atkuriami](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)elementai esančių elementų naikinimas.

Norėdami išvengti aplanko Atkuriami elementai visiško, administratoriai gali padidinti sulaikytų pašto dėžučių aplanko Atkuriami elementai saugyklos limitą ir nustatyti pašto dėžutės saugojimo strategiją, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo pašto dėžutę. Žr. [Sulaikytų pašto dėžučių atkuriamų elementų kvotos didinimas.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
