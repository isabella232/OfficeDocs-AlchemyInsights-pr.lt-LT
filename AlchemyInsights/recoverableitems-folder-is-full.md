---
title: 1336 RecoverableItems aplankas yra pilnas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510760"
---
# <a name="the-recoverable-items-folder-is-full"></a>Atkuriamų elementų aplankas pilnas

Exchange Online pašto dėžučių, numatytasis saugyklos riba atkuriamų elementų aplanko yra 30 GB. Atkuriamų elementų aplanko saugyklos limitas automatiškai padidinamas iki 100 GB, jei pašto dėžutė yra sulaikytas bylinėjimosi, el. duomenų aptikimo sulaikymas arba priskirtas saugojimo strategijai.

Kai atkuriamų elementų aplankas pasiekia saugyklos ribą, pašto dėžutės funkcija turi įtakos šiais būdais:

- Vartotojas negali panaikinti elementų iš pašto dėžutės.

- Valdomojo aplanko asistentas negali panaikinti elementų pagal saugojimo žymę arba valdomo aplanko parametrus.

- Pašto dėžučių, kuriose įgalintas vieno elemento atkūrimas arba kurios yra sulaikytos, kopijavimo rašymo puslapio apsaugos procesas negali išlaikyti vartotojo redaguotų elementų versijų.

- Pašto dėžučių, kuriose įgalintas pašto dėžučių audito registravimas, nėra pašto dėžutės audito žurnalo įrašus galima įrašyti į aplanką Atkuriami elementai poaplankyje Audito.

Pašto dėžučių, kurios nėra sulaikytas, administratoriai gali naudoti `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandą Exchange Online PowerShell panaikinti elementus į atkuriami elementai aplanke. Norėdami gauti daugiau informacijos žr. toliau nurodytas temas:

- [Pranešimų ieška ir naikinimas](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Ieškos pašto dėžutė](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Sulaikytoms pašto dėžutėms administratoriai turi pašalinti sulaikymą, kad galėtų panaikinti elementus iš aplanko Atkuriami elementai. Daugiau informacijos [ieškokite Naikinti elementus, esančius nuotolinių išteklių saugyklomis pagrįstų pašto dėžučių aplanke Atkuriami elementai](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Kad aplankas Atkuriami elementai netaptų pilnas, administratoriai gali padidinti sulaikytų pašto dėžučių aplanko Atkuriami elementai saugyklos ribą ir nustatyti pašto dėžutės saugojimo strategiją, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo pašto dėžutę. Peržiūrėkite [padidinti sulaikytų pašto dėžučių atkuriamų elementų kvotą](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
