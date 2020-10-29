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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801559"
---
# <a name="attack-simulator-in-microsoft-365"></a>"Microsoft 365" atakos simuliatorius

- Ar trūksta atakos treniruoklio? Atakos simuliatorius reikalauja **"Microsoft Defender" "office 365" plano 2 (ATP 2 planas) arba "** **Office 365 Enterprise E5** ". Atakos **simuliatorius neįtrauktas į** "Microsoft Defender", skirtą "Office 365" 1 planas (ATP 1 planas), "Office 365 Enterprise E3" arba bet kurią "Microsoft 365" verslui prenumeratų taikomąsias programas.

- Paskyrai, kurią naudojate norėdami inicijuoti modeliuojamoms atakoms, reikia visuotinių administratoriaus ar saugos administratoriaus teisių ir kelių dalių autentifikavimo (MFA). Daugiau informacijos apie atakos imitatoriaus reikalavimus rasite [šioje temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Svarbūs dalykai, kuriuos reikia žinoti apie **brute force slaptažodžio** atakos modeliavimą:

  - Jei paskirties paskyroje įgalinta MFA ir slaptažodis buvo tinkamai atspėtas, paskyra nebus rodoma kaip pažeista (antrasis autentifikavimo faktorius bus neišsamus).

  - Slaptažodžio failas negali būti didesnis nei 10 MB. Naudokite vieną slaptažodį eilutėje ir įtraukite tuščią eilutę (grįžties mygtuką) po paskutinio slaptažodžio sąraše.

- Svarbūs dalykai, kuriuos reikia žinoti apie " **Spear phishing** " pridėti modeliavimų:

  - Pagal dizainą negalite pateikti " **phishing" prisijungimo serverio URL** pasirinktinio reikšmės.

  - Jei gavėjas naudoja [ataskaitos pranešimo priedą įgalinti](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , kad pranešimas būtų praneštas kaip sukčiavimas apsimetant, galite negauti pranešimo įspėjimų (nes tai sumodeliuotas išpuolis).

- Ataskaitos: po modeliuojamos atakos, galite spustelėti **atakuoti informaciją** , kad matytumėte ataskaitą.

- Išsamių instrukcijų ir naujų funkcijų atakos simuliatoriuje ieškokite ["Microsoft 365" atakos simuliatorius](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
