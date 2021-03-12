---
title: Sąlyginė prieiga su Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704794"
---
# <a name="conditional-access-with-intune"></a>Sąlyginė prieiga su Intune

Naudojant  **sąlyginę prieigą**  su Intune reikia 3 veiksmų:

- Sukurkite  **atitikties strategiją**  (["Android](https://docs.microsoft.com/intune/compliance-policy-create-android)", "  [ios](https://docs.microsoft.com/intune/compliance-policy-create-ios)",  ["Windows"](https://docs.microsoft.com//intune/compliance-policy-create-windows)), kad nustatytumėte parametrus, kuriuos reikia atitikti prieš tai, kai prietaisas laikomas atitinkančiu reikalavimus. Pvz., įrenginyje turi būti bent 6 skaitmenų PIN, kad jis būtų laikomas atitinkančiu reikalavimus.
- Sukurkite **sąlyginės prieigos strategiją**  , kuri apibrėžia, kokie ištekliai yra saugomi, ir kokiomis sąlygomis reikia pasiekti šiuos išteklius.  [Pavyzdžiui,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  įrenginys turi būti suderinamas prieš jungiantis prie įmonės elektroninio pašto.
- Užtikrinkite, kad **atitikties strategijos**  ir  **sąlyginės prieigos strategijos**  būtų nukreiptos į pageidaujamas vartotojų grupes. Tam gali reikėti sukurti tam tikras vartotojų grupes "Azure Active Directory".

**Naudingi saitai:**

[Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)

[Trikčių diagnostika CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Trikčių šalinimo strategija](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Norint apsaugoti el. paštą ("Exchange Online") iš "Access" neatitinkančius įrenginius, būtina laikytis abiejų dokumentų:

1. [El. pašto prieigos apsauga iš įrenginių, naudojančių EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Apsaugoti pašto prieigą iš įrenginių, naudojančių šiuolaikinius autentifikavimo klientus, pvz., "Outlook"](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)