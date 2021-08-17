---
title: 2681 attack Simulator in Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895799"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Ar jums trūksta atakos simuliatoriaus? "Attack Simulator" **reikia "Microsoft" sargybos Office 365 2 arba** **Office 365 Enterprise E5.** Atakos **simuliatorius** neįtrauktas į "Microsoft" sargybą, Office 365 1 planą, "Office 365 Enterprise E3" arba "Microsoft 365" programos verslui prenumeratas.

- Paskyrai, kurią naudojate imituoties atakoms paleisti, reikia visuotinio administratoriaus arba saugos administratoriaus teisių ir kelių dalių autentifikavimo (MFA). Daugiau informacijos apie atakos simuliatoriaus reikalavimus žr. [šioje temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Svarbūs dalykai, kuriuos reikia žinoti apie **"Brute Force Password"** atakos modeliavimą:

  - Jei paskirties paskyroje įgalintas MFA ir slaptažodis buvo atspėjamas tinkamai, paskyra nebus rodoma kaip pažeista (antrasis autentifikavimo koeficientas bus neišsamus).

  - Slaptažodžio failas negali būti didesnis nei 10 MB. Naudokite vieną slaptažodį vienoje eilutėje ir įtraukite tuščią eilutę (gabenimo grąžinimą) po paskutinio sąrašo slaptažodžio.

- Svarbūs dalykai, kuriuos reikia žinoti apie **sukčiavimo apsimetant pridėjimo** modeliavimą:

  - Pagal dizainą negalite pateikti pasirinktinės reikšmės apsimestinių duomenų **registravimosi serverio URL.**

  - Jei gavėjas [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) naudoja ataskaitos pranešimo papildinyje įgalinti pranešimą kaip sukčiavimą apsimetant, galite negauti įspėjimų apie pranešimą (nes tai yra imituota ataka).

- Ataskaitos: kai imituota ataka bus baigta, galite spustelėti **Atakos išsami informacija,** kad pamatytumėte ataskaitą.

- Išsamias instrukcijas ir naujas "Attack Simulator" funkcijas žr. [Atakos simuliatorius Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
