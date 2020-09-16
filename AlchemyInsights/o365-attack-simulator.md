---
title: 2681 atakos simuliatorius programoje "Microsoft 365"
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759227"
---
# <a name="attack-simulator-in-microsoft-365"></a>"Microsoft 365" atakos simuliatorius

- Ar trūksta atakos treniruoklio? Atakos treniruokliui reikia " **office 365" išplėstinės grėsmės apsaugos plano 2 (ATP planas 2)** arba " **Office 365 Enterprise E5**". Atakos simuliatorius **nėra** įtrauktas į "Office 365" išplėstinės grėsmės apsaugos planą 1 (ATP planas 1), "Office 365 Enterprise E3" arba bet kurias "Microsoft 365" taikomąsias programas verslui prenumeratos.

- Paskyrai, kurią naudojate norėdami inicijuoti modeliuojamoms atakoms, reikia visuotinių administratoriaus ar saugos administratoriaus teisių ir kelių dalių autentifikavimo (MFA). Daugiau informacijos apie atakos imitatoriaus reikalavimus rasite [šioje temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Svarbūs dalykai, kuriuos reikia žinoti apie **brute force slaptažodžio** atakos modeliavimą:

  - Jei paskirties paskyroje įgalinta MFA ir slaptažodis buvo tinkamai atspėtas, paskyra nebus rodoma kaip pažeista (antrasis autentifikavimo faktorius bus neišsamus).

  - Slaptažodžio failas negali būti didesnis nei 10 MB. Naudokite vieną slaptažodį eilutėje ir įtraukite tuščią eilutę (grįžties mygtuką) po paskutinio slaptažodžio sąraše.

- Svarbūs dalykai, kuriuos reikia žinoti apie " **Spear phishing** " pridėti modeliavimų:

  - Pagal dizainą negalite pateikti " **phishing" prisijungimo serverio URL**pasirinktinio reikšmės.

  - Jei gavėjas naudoja [ataskaitos pranešimo priedą įgalinti](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , kad pranešimas būtų praneštas kaip sukčiavimas apsimetant, galite negauti pranešimo įspėjimų (nes tai sumodeliuotas išpuolis).

- Ataskaitos: po modeliuojamos atakos, galite spustelėti **atakuoti informaciją** , kad matytumėte ataskaitą.

- Išsamių instrukcijų ir naujų funkcijų atakos simuliatoriuje ieškokite ["Microsoft 365" atakos simuliatorius](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
