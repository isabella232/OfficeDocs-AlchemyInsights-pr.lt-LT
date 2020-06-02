---
title: 2681 Ataka simuliatorius Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506746"
---
# <a name="attack-simulator-in-microsoft-365"></a>Ataka simuliatorius Microsoft 365

- Ar jums trūksta ataka simuliatorius? Atakos modeliuoklis reikalauja **"Office 365" išplėstinio apsaugos nuo grėsmių plano 2 (ATP 2 planas)** arba **"Office 365 Enterprise E5".** "Attack Simulator" **neįtrauktas** į "Office 365" saugos nuo grėsmių planą (ATP 1 planas), "Office 365 Enterprise E3" arba "Microsoft 365" programas verslui.

- Abonementui, kurį naudojate imituojamoms atakoms paleisti, reikia visuotinio administratoriaus arba saugos administratoriaus teisių ir kelių dalių autentifikavimo (DTS). Daugiau informacijos apie atakos simuliatoriaus reikalavimus rasite [šioje temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Svarbūs dalykai, kuriuos reikia žinoti apie **Brute Force Password** attack modeliavimas:

  - Jei paskirties abonementas įgalintas Ir slaptažodis buvo atspėjote teisingai, abonementas nebus rodomas kaip pažeistas (antrasis autentifikavimo koeficientas bus nebaigtas).

  - Slaptažodžio failas negali būti didesnis nei 10 MB. Naudokite vieną slaptažodį eilutėje ir po paskutinio sąrašo slaptažodžio įtraukite tuščią eilutę (vežimėlio grąžinimą).

- Svarbūs dalykai, kuriuos reikia žinoti apie **ietis Phishing** pridėti modeliavimas:

  - Pagal dizainą negalite pateikti pasirinktinės **apsimestinių svetainių prisijungimo serverio URL**reikšmės.

  - Jei gavėjas naudoja [ataskaitos pranešimo priedo įgalinimą](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pranešimui pranešti kaip apie sukčiavimą, galite negauti pranešimo įspėjimų (nes tai imituojamas ataka).

- Ataskaitos: kai imituojamas ataka bus baigta, galite **spustelėti Išsami ataka,** kad pamatytumėte ataskaitą.

- Išsamių atakos simuliatoriaus instrukcijų ir funkcijų ieškokite ["Attack Simulator" programoje "Microsoft 365".](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
