---
title: 1336 RecoverableItems aplankas yra visiškai
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: a048949d5284d018303d03aad26cdf26eee2fb5c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776404"
---
# <a name="the-recoverable-items-folder-is-full"></a>Aplanko Atkuriami elementai yra visiškai

Exchange Online pašto dėžutes "Office 365", numatytosios saugyklos aplanko Atkuriami elementai yra 30 GB. Saugyklos aplanko Atkuriami elementai automatiškai padidinama iki 100 GB skiriamas sulaikymas dėl bylinėjimosi, eDiscovery laikyti, ar priskirtas "Office 365" saugojimo strategijos pašto dėžutės.
  
Aplanko Atkuriami elementai pasiekus saugyklos ribą, pašto dėžutės funkcijas veikia vienu iš šių būdų:
  
- Vartotojas negali panaikinti elementus iš pašto dėžutės.
    
- Valdomojo aplanko asistentas negali naikinti elementus saugojimo žymę arba valdomojo aplanko parametrai.
    
- Pašto dėžučių, kurios vieno elemento atkūrimas įgalintas arba yra laikinieji, kopija rašant puslapis apsaugos procesas negali išlaikyti prekių vartotojas redagavo versijas.
    
- Pašto dėžučių ar pašto dėžutės audito žurnalo pildymo funkcija įjungta, pašto dėžutės audito žurnalo įrašai gali būti saugomi audito poaplankį aplanke Atkuriami elementai.
    
Pašto dėžučių, kuris nėra sulaikytas, administratoriai gali naudoti ir `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komanda Exchange Online "PowerShell" Norėdami naikinti elementus aplanke Atkuriami elementai. Norėdami gauti daugiau informacijos žr. toliau nurodytas temas: 
  
- [Ieškoti ir panaikinti laiškus](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Paieška-dėžutės](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Pašto dėžučių, kurios yra sustabdytos, administratoriai turi pašalinti sulaikymą, kol jie gali panaikinti elementus iš aplanko Atkuriami elementai. Daugiau informacijos rasite [Naikinti elementus aplanke nuotolinių išteklių saugyklomis pagrįstos pašto dėžučių laikykite Atkuriami elementai](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Siekiant padėti užkirsti kelią aplanko Atkuriami elementai tampa pilna, administratoriai gali padidinti atkuriamų elementų aplanko pašto dėžutės palaikykite ir nustatyti pašto dėžutės saugojimo strategija, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo saugyklos pašto dėžutės. Peržiūrėkite [padidinti Atkuriami elementai kvota pašto dėžučių, laikykite](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

