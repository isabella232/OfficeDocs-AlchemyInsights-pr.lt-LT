---
title: 2681 ataka simuliatorius Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305339"
---
# <a name="attack-simulator-in-office-365"></a>Ataka simuliatorius Office 365

- Ar jums trūksta Attack Simulator? Attack Simulator reikia **office 365 Išplėstinė grėsmės apsaugos planas 2 (ATP planas 2)** arba **Office 365 Enterprise E5**. Attack Simulator nėra **įtraukta į** Office 365 Išplėstinė grėsmės apsaugos planas 1 (ATP planas 1), Office 365 Enterprise E3 arba bet kuri Office 365 verslo prenumeratos.

- Abonementą, kurį naudojate pradėti imituoti atakų reikia visuotinio administratoriaus arba saugos administratoriaus teises ir kelių dalių autentifikavimas (DTS). Daugiau informacijos apie "Attack Simulator" reikalavimus rasite [šioje temoje](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Svarbūs dalykai, kuriuos reikėtų žinoti apie **brute force slaptažodis** ataka modeliavimas:

  - Jei paskirties abonementas yra įgalintas DTS ir slaptažodis buvo atspėti teisingai, sąskaitos nebus rodomas kaip pavojus (antrasis autentifikavimo koeficientas bus nebaigtas).

  - Slaptažodžio failas negali būti didesnis nei 10 MB. Kiekvienai eilutei naudokite vieną slaptažodį ir įtraukite tuščią eilutę (vežimėlio grąžinimas) po paskutinio slaptažodžio sąraše.

- Svarbūs dalykai, kuriuos reikėtų žinoti apie **Spear phishing** pridėti modeliavimas:

  - Pagal dizainą negalite pateikti **apsimestinių svetainių prisijungimo serverio URL**pasirinktinės reikšmės.

  - Jei gavėjas naudoja pranešimą [įgalinti priedą pranešti](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , kad pranešimas būtų naudojamas kaip sukčiavimas apsimetant, gali būti, kad negaunate pranešimo įspėjimų (nes tai imituojamas ataka).

- Ataskaitos: po to, kai imituojamas ataka yra baigtas, galite spustelėti **ataka detalės** Norėdami pamatyti ataskaitą.

- Išsamias instrukcijas ir naujų funkcijų ataka simuliatorius, žr [ataka simuliatorius Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
