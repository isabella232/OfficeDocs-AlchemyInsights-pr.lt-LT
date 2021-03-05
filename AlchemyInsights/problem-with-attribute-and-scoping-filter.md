---
title: Problema su atributo ir aprėpties filtru
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481895"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problema su atributo ir aprėpties filtru

**Problema dėl nesuderinamų UPN reikšmių**

Darbo dienos iki skelbimo vartotojo parengimo darbo dienos iki skelbimo vartotojo parengimo rodomas klaidos pranešimas **Hybridsynchronizationactivedirectoryuserprincipalnamenotunique**. Operacija nepavyko dėl to, kad į sudėties/Modifikacijos reikšmė nėra unikali. Išsami klaidos informacija: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

" **UserPrincipalName** " reikšmė, kurią bando nustatyti, kai kuriamas skelbimo vartotojo abonementas jau yra paskirties skelbimų srityje. Tai reiškia, kad (1) vartotojas jau yra ir atitikimo ID žymės nepavyko vartotojui arba (2) UPN generavimo taisyklė sugeneravo nesuderinamą reikšmę.

Pateikiame siūlomus sprendimo veiksmus:

Jei vartotojas jau yra, o atitikimo ID patikra nepavyko susieti darbo dienos paskyros su "Active Directory" paskyra, tada patikrinkite, ar atitikimo ID atributas (paprastai **darbuotojai**) tiek darbo dieną, tiek AD turi tikslią atitiktį. Jei jie neturi atitikmens, tai yra duomenų problema, kurią reikia išspręsti. Pavyzdžiui, jei "darbuotojai" yra "001052" ir skelbime ji yra 1052, tada parengimo modulis nepavyks susieti dviejų paskyrų ir bandys sukurti jau esamą vartotoją. Šiuo atveju sprendimas yra pakeisti **darbuotojai** reikšmę skelbime, kad būtų įtraukti nuliai, kad jis 001052.
Jei "UPN" generuojama išraiška nesugeneruoja unikalios reikšmės, **Apsvarstykite galimybę naudoti funkciją de** -dubliavimo, kad kiekvieną kartą sukurtumėte unikalią reikšmę.

**Darbo dienos į skelbimų vartotojo parengimas nenustatė vadovo atributo reikšmė, skirta skelbimų vartotojo abonementui**

"WORKDAY to AD" vartotojo parengimo užduotis nėra parametro **vadovo** atributo reikšmė. Yra du galimi scenarijai, kai šis elgesys yra matomas:

1. Darbo dienos tvarkytuvas negali būti išspręstas atitinkamam skelbimo vartotojo abonementui, nes vadovo nėra aprėpties.
2. **Kelių skelbimų domenų** scenarijuje, darbo dienos tvarkytuvas nėra tame pačiame domene kaip vartotojas.

Išbandykite šiuos veiksmus, kad išspręstumėte problemą:

1. Jei nustatėte aprėpties filtrus, pirmiausia patikrinkite, ar tvarkytuvas yra aprėpties ir ar jis atitinka sąlygą aprėpties. Jei vadovas neatitinka aprėpties filtro, pakeiskite filtrą taip, kad vadovas taip pat aprėptų parengimo operaciją.
2. Jei turite kelis skelbimų domenus, tada jungiamoji dalis turi žinomą nesugebėjimo išspręsti kelių domenų vadovo nuorodas apribojimą.

Išsamesnės informacijos apie darbo dienos konfigūravimą automatiniam parengimas ieškokite straipsnyje [Susipažinkite: darbo dienos konfigūravimas automatiniam vartotojų parengimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













